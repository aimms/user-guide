.. _option-SNOPT-major_step_limit:


Major Step Limit
================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	2.0	



This option limits the change in x during a line search. It applies to all nonlinear problem, once a "feasible solution" or "feasible subproblem" has been found.



A line search determines a step a over the range 0 < a <= b, where b is 1 if there are nonlinear constraints, or the step to the nearest upper or lower bound on x if all the constraints are linear. Normally, the first steplength tried is a1 = min(1, b).



In some cases, such as f(x) = aebx or f(x) = axb, even a moderate change in the components of x can lead to floating-point overflow. The value of this option is therefore used to define a limit



b' = r (1``+ ||x||``)``/ ||p||`` ``,`` 



(where r is the major step limit and p the search direction), and the first evaluation of f(x) is at the potentially smaller steplenth a1 = min(1, b', b).



Whenever possible, upper and lower bounds on x should be used to prevent evaluation of nonlinear functions at meaningless points. This option provides an additional safeguard. The default setting of 2.0 should not affect progress on well behaved problems, but setting its value to 0.1 or 0.01 may be helpful when rapidly varying functions are present. A "good" starting point may be required. (An important application is the class of nonlinear least-squares problems.)



In cases where several local optima exist, specifying a small value may help to locate an optimum near the starting point.



