

.. _Baron_General_-_Maximal_variable_bound:


Maximal variable bound
======================



:Type:	Floating point number	
:Range:	[0.0,1e51]	
:Default:	1e50	



If a variable has no upper bound then the upper bound passed to BARON will be equal to the value of this option. If a variable has no lower bound then the lower bound passed to BARON will be equal to the value of this option multiplied by -1.



For example, if you have a variable x1 with range [0,999999] and a variable x2 with range [0,inf) then this will be passed to BARON as variables x1 with range [0,999999] and x2 with range [0,1000] if the value of this option is set to 1000.



If the value of this option is set to 1e50 (or higher) then each infinite variable bound in AIMMS will be treated as an infinite variable bound by BARON. This is the default setting.



**Note** 

*	BARON requires that all nonlinear variables and expressions in the mathematical program are bounded from below and above. It is important that the user provides finite lower and upper bounds on the variables. If not, global optimality of the solution provided is sometimes not guaranteed.
*	BARON might return 'infeasible' if the value of this option is set too low.
*	If you think that BARON does not return a global optimal solution for your model, you might consider increasing the value of this option.
*	In BARON version 10.3 and older the default of this option was 1000.



