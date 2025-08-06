

.. _CONOPT_Troubleshooting:
.. _CONOPTTroubleshooting:


Troubleshooting
===============

**CONOPT returns (locally) infeasible** 

If CONOPT reports that the model is 'locally infeasible' it can be that the model is really infeasible or that CONOPT fails to solve the (feasible) model for some reason. You should first use the AIMMS Nonlinear Presolver because it can often detect whether a model is really infeasible and it can give additional information that might help you understand why the model is infeasible. To do so you should switch on the general solvers option **Nonlinear Presolve** . To print the infeasibility analysis to the listing file you should also switch on the general solvers option **Display Infeasibility Analysis** .



If CONOPT reports that the model is 'locally infeasible' (and the AIMMS Nonlinear Presolver did not detect that your model is infeasible) you should check the Message Window (opened by pressing 'Ctrl'+'m') to see if additional information has been printed there. The Message Window might show one of the following messages:



1.	CONOPT found error in row constraint-name: All Jacobian elements in the row are very small.

2.	CONOPT found error in nonzero in row constraint-name and column variable-name: Jacobian element too large = value.

3.	CONOPT found error in row constraint-name: Slack has reached internal 'Infinity'.



**Cas** **e 1: All Jacobian elements in the row are very small** 

In the first case, all first-order derivatives (i.e., the Jacobian elements) in the reported constraint are close to 0. For example, if the constraint has a definition



X * Y + U * V <= 100,



where X, Y, U and V are nonnegative variables, then CONOPT might show the first error message if all 4 variables are initialized to 0. To repair this situation you could try one of the following suggestions:




*   Set the lower bound of a variable in the constraint to a value such that at least one of the first-order derivatives cannot become 0 anymore. In the example you could set X.lower := 0.0001;
*   Set the initial value of a variable in the constraint to a value such that at least one of the (initial) first-order derivatives will be unequal to 0. In the example you could set X.level := 10;



**Cas** **e 2: Jacobian element too large** 

In the second case, the first-order derivative for the reported constraint-variable combination becomes too large. For example, if the constraint has a definition



1.0e6 * X + Y >= 1.0e6,



where X and Y are nonnegative variables, then CONOPT might show the second error message if the value of X becomes too large. To repair this situation you could try one of the following suggestions:




*   Scale the constraint. In the example you could divide all coefficients by 1000 to get the definition 1.0e3 * X + 1.0e-3 * Y >= 1.0e3.
*   Set the upper bound of the variable to a value such that the first-order derivative cannot become large anymore. In the example you could set X.upper := 2.0;
*   Set the initial value of the variable to a value such that the initial first-order derivative becomes small. In the example you could set X.level := 0.001;



**Cas** **e 3: Slack has reached internal 'Infinity'** 

In the third case, the difference between the left hand side and the right hand side of the constraint has become too large at one point in the solution process. This might be the case if the right hand side value is very large. For example, if the constraint has a definition



X + Y <= 1.0e8,



then CONOPT might show the third error message if X and Y are close to 0. To repair this situation you could try one of the following suggestions:




*   Scale the constraint. In the example you could divide all coefficients by 1000 to get the definition 1.0e-3 * X + 1.0e-3 * Y <= 1.0e5.
*   Increase the value of the option **Maximal Solution of a Variable** . This should only be done if the other suggestion fails.



**Learn more about** 

*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 
*	:ref:`Options_NonlinPres_-_DisplayInfyAnalys` 
*	:ref:`CONOPT_Limits_-_Maximal_Solution_Variable` 



