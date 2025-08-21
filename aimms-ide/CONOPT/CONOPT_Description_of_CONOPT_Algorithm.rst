

.. _CONOPT_Description_of_CONOPT_Algorithm:
.. _CONOPTDescription_of_CONOPT_Algorithm:


Description of CONOPT Algorithm
===============================

**Preprocessor** 

CONOPT 4 distinguishes between a 'user model' as defined by the user via the AIMMS language, and an 'internal model'. Pre-triangular variables and constraints are simply removed from the user model. Post-triangular variables and constraints are collapsed into a single condensed objective function. And definitional constraints are eliminated. After the internal model has been solved CONOPT translates the internal solution back into the solution for the user model and reports this solution to the user.



In addition to the simple pre- and post-triangular variables and constraints, the preprocessor in CONOPT looks at more possibilities for simplifying the model. Some of the new features are:




*   Fixed variables are removed completely.
*   Constraints that represent simple inequalities are identified and changed into simple bounds on the variables and the constraints are removed.
*   Simple monotone constraints such as exp(x) <= c1 or log(y) <= c2 are converted into simple bounds on the variables and then removed.
*   Forcing constraints such as x1 + x2 <= 0 with x1.lower = 0 and x2.lower = 0 are identified, the variables are fixed, and the constraints are removed. If a forcing constraint is identified then other constraints may become pre-triangular so they also can be removed.
*   Linear and monotone constraints are used to compute 'implied bounds' on many variables and these bounds can help CONOPT get a better starting point for finding an initial feasible solution.
*   Some non-monotone constraints such as sqr(x1) + sqr(x2) <= 1 can also be used to derive implied bounds (here -1 < x1 < +1 and -1 < x2 < +1) that both can improve the starting point and can be used to determine that other terms are monotone.
*   Constraints with exactly two variables, e.g. simple linear identities such as x1 = a*x2 + b or simple monotone identities such as x3 = exp(x4), are used to move bounds between the two variables and this may result in more variables being included in the post-triangle.
*   Linear constraints that are identical or proportional to others are identified and removed.
*   Pairs of constraints that define a lower and an upper bound on the same linear expression or proportional linear expressions, e.g. 1 <= x1 + x2 and 2*x1+2*x2 <= 4, are turned into a single ranged constraint implemented with a double-bounded slack variable.
*   Nonlinear constraints that become linear when the pre-triangular variables are fixed are recognized as being linear with the resulting simplifications.



The preprocessor also identifies constructs that are easy to make feasible. There are currently two types:




*   Penalty terms: We define a penalty constraint as a constraint of the form f(x1,x2,..) + p - n = 0, where p and n are positive variables, and where p and n only appear in post-triangular constraints or in previously identified penalty constraint. For any feasible values of the x-variables it is easy to find values of p and n that makes the penalty constraint feasible: p = max(0,-f(x)) and n = max(0,f(x)). The definition is easily generalized to constraints where p and n have coefficients different from one and nonzero bounds; the essence is the presence of two linear unbounded terms of opposite sign.
*   Minimax terms: We define a minimax group as a group of constraints of the form eq(i).. fi(x1,x2,..) <= z where z is common to the group and otherwise only appear in post-triangular constraints, and z is unbounded from above. For any feasible value of the x-variables it is easy to find a value of z that makes the minimax group feasible: z = smin(i: fi(x)). The definition is easily generalized to groups of constraints where z has coefficients different from one and where the direction of the inequality is reversed.



The preprocessor will also recognize definitional equations: constraints of the form x = f(y), where x is a free variable or the bounds on x cannot be binding, are called definitional equations and x is called a defined variable. If there are many potential defined variable the preprocessor will select a recursive set and logically eliminate them from the internal model: The values of the defined variables are easily derived from the values of all other variables by evaluating the definitional equations in their recursive order, and these values are substituted into the remaining constraints before their residuals are computed. The matrix of derivatives of the remaining constraints is computed from the overall matrix of derivatives via an elimination of the triangular definitional equations. The definitional equations are eliminated from the internal model and they are not present in the internal operations used to solve this model. For some models this can make a big difference.



The preprocessor can be switched off by disabling the option **Preprocessor** .



**Phase 0 - Finding an Initial Feasible Solution** 

Phase 0 is started with a new 'Adjust Initial Point' procedure that tries to minimize the sum of infeasibilities by changing individual variables one at a time. The procedure is very cheap since each change of a single variable only involve a small part of the overall model, and it will as a by-product produce a large part of a good initial basis and many constraints will become feasible. The procedure can in some cases reduce the sum of infeasibilities significantly.



CONOPT uses a rigorous LP framework in Phase 0 that iteratively finds a better basis for Newton's method. CONOPT can therefore be slower for very easy models but the variability in solution time is smaller and it should never be very slow.



**Bad Iterations** 

Bad iterations (flagged with “F” in the “OK” column of the CONOPT status file) are an important problem for CONOPT. They appear if the output from the SLP or SQP procedure is a search direction where CONOPT cannot move very far because it is difficult to make the nonlinear constraints feasible again. The efforts spend in solving the SLP or SQP procedure is therefore partially wasted. The problem is usually associated with a basis that is ill-conditioned or changes very fast.



CONOPT uses a rigorous procedure based on monitoring the size of some intermediate terms. It can be the size of elements of the tangent for basic variables relative to similar elements for superbasic variables. Or it can be intermediate results from the computation of the reduced costs. The monitoring procedure is cheap and it is used to maintain a well-conditioned basis throughout the optimization instead of waiting until something does not work well.



The transition from SLP to SQP and back again is based on continuous measurements of curvature, both in the general constraints and in the objective function, combined with estimates of computational costs and progress for SLP and SQP.



**Saddle Points and Directions of Negative Curvature** 

CONOPT is based on moving in a direction derived from the gradient (or the reduced gradient for models with constraints). If the reduced gradient (projected on the bounds) is zero then the solution satisfies the first-order optimality conditions and it is standard procedure to stop. Unfortunately, this means that we can stop in a saddle-point.



It is not very common to move towards a saddle-point and get stuck in it. However, it is not uncommon that the initial point, provided by a user or by default, is a saddle point. A simple example is the constraint x*y = 1 started with x = y = 0 that easily can end with a locally infeasible solution. Or minimize z, z = x*y with the same starting point that could end locally optimal without moving even though better points exist in the neighborhood.



CONOPT has an added procedure that tries to find a direction of negative curvature that can move the solution point away from a saddle-point. The procedure is only called in points that satisfy the first order optimality conditions and it is therefore a cheap safeguard. The theory behind the method is developed for models without degeneracy and it works very well in practice for these models. Models with some kind of degeneracy (basic variables at bound or nonbasic variables with zero reduced cost) use the same procedure, but it is in this case only a heuristic that cannot be guaranteed to find a direction of negative curvature, even if one exists.



If the model is known to be convex you can switch on the option **Model is Convex**  which will turn this procedure off. The saving is usually very small, except for models that solve in very few iterations and for model with a large number of superbasics.



There is no output in the CONOPT status file for negative curvature. If a useful direction is found CONOPT will follow it and the optimization continues. Otherwise, the solution is declared locally optimal.



**Use of Alternative Sub-Models** 

During the course of an optimization CONOPT can work with up to three different internal sub-models. These models are:




*   **Full Model** : This model consists of the constraints in the user's model excluding all pre- and post-triangular constraints and with the definitional variables eliminated by their defining constraints.
*   **No-Penalty Model** : This model consists of the Full Model excluding all penalty and mini-max constraints. This model does not have an objective function.
*   **Linear Feasibility Model** : This model consists of the linear constraints of the Full Model. The Linear Feasibility model is either solved without an objective function or minimizing a quadratic distance measure; this is discussed below.



The pre-triangular variables are considered fixed and they do not appear in any of the sub-models. Their influence comes through their contribution to coefficients and constant terms. The post-triangular variables are considered intermediate variables in the definition of the objective function. They do not appear in the last two models that only are concerned with feasibility, and they only appear indirectly via the objective in the Full Model. The defined variables are considered intermediate variables in the definition of the remaining constraints in the same way as post-triangular variables are intermediate in the objective. The variables in the Full Model are all variables excluding pre- and post-triangular variables and excluding defined variables; this set can include variables that do not appear in any constraints. The constraints of the full models are all constraints excluding pre- and post-triangular constraints and with the definitional equations logically eliminated. The variables in the Linear Feasibility Model and in the No-Penalty Model are the variables that appear in the constraints of these models (excluding pre-triangular variables).



CONOPT always starts by searching for a feasible solution and the sub-models only play a role in this part of the optimization so if the initial point provided by the modeler is feasible then these sub-models are irrelevant. If there are many penalty and/or minimax constraints then the No-Penalty Model will be much smaller than the Full Model and it is more efficient to use the smaller model while searching for feasibility. So the No-Penalty model is only introduced for efficiency reasons. It is by default solved before the Full Model if all of the following conditions are satisfied:




*   The option **Use No-Penalty Model**  is switched on (the default setting).
*   The user did not provide an initial basis.
*   Some of the constraints in the No-Penalty Model are infeasible.
*   The number of penalty and minimax constraints is more than the number of constraints in the Full Model multiplied by the value of the option **Penalty Constraints Ratio** . The default value of **Penalty Constraints Ratio**  is 0.1, i.e. the No-Penalty Model is only defined and solved if it is at least 10% smaller than the Full Model.



**The Linear Feasibility Model** 

The Linear Feasibility Model is introduced to help avoid locally infeasible solutions. It produces a starting point to the nonlinear models (No-Penalty Model or Full Model) that satisfies all linear constraints. If the Linear Feasibility Model is infeasible then the overall model is proved to be infeasible (independent of nonlinearities) and there is no reason to proceed with the nonlinear part of the model.



The Linear Feasibility Model is only useful if the model has some linear constraints and if the initial point provided by the modeler does not satisfy these constraints. If a feasible solution to the linear constraints is found there are several possible ways to continue before the No-Penalty Model and/or the Full Model are started:




#.  Use the solution point as is.




#.  Perform an approximate minimization of the weighted distance from the user's initial point. Include only the variables that have non-default initial values, i.e. variables with an initial value (xini) that is different from zero projected on the bounds, i.e. xini <> min(max(0,x.lower),x.upper). The distance measure is sqr( (x-xini) / max(1,abs(xini)) ).




#.  As in B, but include all variables in the distance measure.




#.  As in C, but define xini to 1 projected on the bounds for all variables with default initial value.



Possibility A is fast but may give a starting point for the nonlinear model far from the initial point provided by the user, B is slower but gives a starting point for the nonlinear model that is close to the point provided by the user, and C and D are also slower but may provide reasonably good and different starting points for the nonlinear model.



The order in which the sub-models are solved depends on a Linear Feasibility Model strategy option, namely the option **Method for Linear Feasibility Models**  which can have the following values:



Method 1 (default):

The initial point and basis is assumed to be fairly good and CONOPT4 will start with the No-Penalty Model (only if the conditions mentioned above are satisfied) followed by the Full Model. If the model terminates locally optimal, unbounded, or on some resource limit (time, iterations, function evaluations) then we are done and CONOPT terminates. But if the model is locally infeasible then we build and solve the Linear Feasibility Model. If this model is infeasible, the overall model is infeasible and we are again done. If it is feasible we minimize objective B and use the solution point as a second starting point for the nonlinear model. If this attempt also terminates locally infeasible we try to generate an alternative initial point with objective C and then with objective D. If all fails, the model is labeled locally infeasible.



Method 2:

CONOPT will start with the Linear Feasibility Model with objective A before looking at the No-Penalty and Full models. If they are locally infeasible from this starting point we followed the procedure from above with objective B, C, and then D.



Method 3:

This method is similar to 'Method 2' except that the first objective A is skipped.



The number of submodels that are solved is limited by the option **Limit on Linear Feasibility Model Rounds** .



If the model is defined to be convex, by switching on the option **Model is Convex** , then a locally infeasible solution is labeled (globally) infeasible and the Linear Feasibility Model will not be used.



**Multiple Threads** 

CONOPT 4 can use multiple threads for some internal computations and for function and derivative evaluations (through AIMMS). Multiple threads are currently only used for certain fairly large and dense computations and these models are quite rare. In addition, multiple threads have a quite high overhead and they are therefore only useful for fairly large models. Currently the best improvements have been for very large models with more than 100,000 variables or constraints. It is the intention to implement multiple threads into more parts of CONOPT in the future. The amount of threads used by CONOPT is controlled by the option **Thread Limit** .



**Learn more about** 

*	:ref:`option-CONOPT-limit_on_linear_feasibility_model_rounds`  
*	:ref:`option-CONOPT-method_for_linear_feasibility_models` 
*	:ref:`option-CONOPT-model_is_convex` 
*	:ref:`option-CONOPT-penalty_constraints_ratio`  
*	:ref:`option-CONOPT-preprocessor` 
*	:ref:`option-CONOPT-thread_limit` 
*	:ref:`option-CONOPT-use_no-penalty_model`  
