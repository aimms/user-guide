

.. _option-AIMMS-repeat_postsolve:


Repeat Postsolve
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option specifies whether or not the postsolve step should be repeated if after the normal postsolve step still some variables violate their bounds. Possible values of this option are:



    *	On
    *	Off




This option is only used if the option **Postsolve Continuous Variables**  is set to 'Round to nearest bound and resolve LP'. With that setting AIMMS checks whether the solution returned by the solver contains contains some variables that violate their bounds. In that case those variables are fixed on their nearest bound, and the LP problem derived in this way is solved. Normally, as a result we obtain a solution in which all variables satisfy their bounds. However, in some cases it might happen that variables that were inside their bounds before (and therefore were not fixed) are violating a bound after the postsolve. If this option is switched on then AIMMS will do another postsolve iteration in which these variables are also fixed (together with the variables that were fixed before). This process is repeated until all variables satisfy their bounds.





**Note** 

*	Please check the option **Postsolve**  for more information regarding the postsolve step.
*	The repeat postsolve is only supported by CPLEX, Gurobi and COPT.




**Learn more about** 

*	:ref:`option-AIMMS-postsolve` 
*	:ref:`option-AIMMS-postsolve_continuous_variables` 



