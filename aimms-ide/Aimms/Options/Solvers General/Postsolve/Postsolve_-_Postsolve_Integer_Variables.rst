

.. _option-AIMMS-postsolve_integer_variables:


Postsolve Integer Variables
===========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Round integers and resolve LP	


MIP solvers do not round the found values for the integer variables to the nearest integer value. Instead it
returns values which are considered to be integer within the integrality tolerance. This option offers the
possibility to perform some postsolving on the found integer solution concerning rounding of integer values.
Possible values are:

    *	No rounding
    *	Round to integer
    *	Round integers and resolve LP


If the value equals 'No rounding' then the variable values found by the solver are passed directly to AIMMS.

If the value equals 'Round to integer' then the integer variable values found by the solver are rounded
before passing them to AIMMS.

If the value equals 'Round integers and resolve LP' then AIMMS checks whether the solution returned by the solver
contains some integer variables that are not really integer. In that case all integer variables are fixed on the
nearest integer value, and the LP problem derived in this way is solved. As a result we obtain a solution in which
all integer variables have a true integer value.


**Note** 

*	The solving time might increase drastically if the value of this option is set to 'Round integers and resolve LP'.
*	In case the value of this option is set to 'No rounding' or 'Round to integer', still the postsolve step can be executed if the value of the option **MIP Calculate Sensitivity Information** is active. To get sensitivity information, all integer variables have to be fixed and the derived LP problem must be solved.
*	Please check the option **Postsolve** for more information regarding the postsolve step.
*	For :ref:`SolverCBC`, the option **Postsolve**  should be switched on to activate this option.


**Learn more about** 

*	:ref:`option-AIMMS-mip_calculate_sensitivity_information`  
*	:ref:`option-AIMMS-postsolve` 

