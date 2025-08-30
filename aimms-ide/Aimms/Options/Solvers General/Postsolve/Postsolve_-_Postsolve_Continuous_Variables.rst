

.. _option-AIMMS-postsolve_continuous_variables:


Postsolve Continuous Variables
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No rounding	


Solvers allow variables to slightly violate their bounds as specified by the feasibility tolerance. This option offers
the possibility to perform some postsolving on the found solution concerning rounding of values to the nearest bound.
Possible values are:

    *	No rounding
    *	Round to nearest bound
    *	Round to nearest bound and resolve LP


If the value equals 'No rounding' then the variable values found by the solver are passed directly to AIMMS.

If the value equals 'Round to nearest bound' then the variable values found by the solver that violate the bounds, by more than
the **Postsolve Bound Tolerance**, are rounded to the nearest bound before passing them to AIMMS.

If the value equals 'Round to nearest bound and resolve LP' then AIMMS checks whether the solution returned by the solver contains contains
some variables that violate their bounds, by more than the **Postsolve Bound Tolerance**. In that case the violated variables are fixed
on their nearest bound, and the LP problem derived in this way is solved. Normally, as a result we obtain a solution in which all variables
satisfy their bounds. In some cases some new variables might violate a bound, in which case the postsolve step can be repeated as controlled
by the option **Repeat Postsolve**.


**Note** 

*	The solving time might increase drastically if the value of this option is set to 'Round to nearest bound and resolve LP'.
*	Please check the option **Postsolve** for more information regarding the postsolve step.
*	For :ref:`SolverCBC`, the option **Postsolve** should be switched on to activate this option.


**Learn more about** 

*	:ref:`option-AIMMS-postsolve` 
*	:ref:`option-AIMMS-postsolve_bound_tolerance` 
*	:ref:`option-AIMMS-repeat_postsolve` 

