

.. _option-AIMMS-postsolve:


Postsolve
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



When solving a problem, solvers like :ref:`SolverCPLEX`, :ref:`SolverGurobi`, :ref:`SolverCOPT` and :ref:`SolverCBC`
allow variables to slightly violate their bounds as specified by some (feasibility) tolerance. Additionally, when
solving a MIP problem, solvers do not round the found integer variable values to the nearest integer value.
Instead the solver returns values which are considered to be integer within some (integrality) tolerance.
For these reasons AIMMS offers a postsolve step during which integer variables are fixed to the nearest
integer or variables outside their bounds are fixed to the nearest bound. The resulting postsolve problem
is then solved to obtain a truly integer solution or a solution in which all variable values are inside the
bounds. Note that the postsolve problem is always a LP problem.

The postsolve step can also be used to calculate sensitivity information for a MIP problem.

This option specifies whether or not a postsolve step will be performed after solving a LP or MIP problem by
CPLEX, Gurobi, COPT or CBC. Possible values of this option are:

    *	Off
    *	Automatic
    *	On


With the default setting of 'Automatic' the postsolve step will be executed if CPLEX, Gurobi or COPT is used
to solve the problem, and it will not be executed if CBC is used. However, if a lazy constraint callback procedure
is installed, which is only supported by CPLEX and Gurobi, then the postsolve step will only be executed if this
option is set to 'On'.

During the postsolve step AIMMS will first check whether the solution returned by the solver is truly feasible
and integer. If that is the case then the postsolve step is normally finished, i.e., AIMMS will then not solve
the postsolve problem. Otherwise AIMMS will solve the postsolve problem using the same solver as was used to solve
the original LP or MIP problem.

If the postsolve step should calculate sensitivity information for a MIP problem, as controlled by the option
**MIP Calculate Sensitivity Information**, then AIMMS will always solve the postsolve problem to obtain this
information (even if the solution returned by the solver is truly feasible and integer). Note that solvers like
CPLEX, Gurobi, COPT and CBC do not provide sensitivity information for MIP problems because it is (in general)
not available for MIP problems. The sensitivity information calculated during the postsolve step only represents
the sensitivity information for the fixed MIP problem, obtained after fixing the integer variables.

Normally, the problem solved during the postsolve step will be feasible, and the objective value returned will
be equal to the objective value that was found by solving the original problem. If the postsolve problem is
infeasible then AIMMS will use the solution that was found before while solving the original problem. If the
postsolve problem is feasible then AIMMS will use the solution found by solving the postsolve problem.

If the postsolve problem is infeasible then this implies that the solution found by the solver was not reliable although it
was feasible according to the tolerances used by the solver. An infeasible postsolve, or a large gap between the objective
values of the original problem and the postsolve problem, indicates that the problem is ill-conditioned. In either case AIMMS
will generate a warning by default, as controlled by the option **Warning Unreliable Solution**. Ill conditioning can often be
"resolved" by adjusting solver tolerances, e.g., by lowering the values of the options that control the feasibility or the
integrality tolerance. But sometimes it can only be resolved by reformulating the problem to improve the numerical stability.

If the postsolve problem is infeasible then AIMMS can print the irreducible infeasibility set (IIS) by switching on the
option **Infeasibility Finder Postsolve**. Analyzing this IIS can help with improving the robustness of the model.


**Other postsolve options** 


The option **Postsolve Integer Variables** determines how AIMMS will handle integer variables during the postsolve step,
while the option **Postsolve Continuous Variables** determines how continuous variables are handled. The postsolve step
can be used to calculate sensitivity information for the fixed MIP problem that is solved during the postsolve; this is
controlled by the option **MIP Calculate Sensitivity Information**.


**Note** 

*	In case of a user interrupt or when the iteration limit is exceeded, the postsolve step might be skipped, depending on the setting of the option **Do Postsolve after Interrupt**.
*	Switching off this option is equivalent to setting the options **Postsolve Continuous Variables** and **Postsolve Integer Variables** to 'No rounding', and the option **MIP Calculate Sensitivity Information** to 'Off'.
*	In case of a MIP problem, solving the postsolve problem can be enforced by switching on the option **MIP Calculate Sensitivity Information**, even if the solution returned by the solver is truly feasible and integer.
*	The postsolve step will always be skipped if CPLEX or Gurobi is used to solve a multi-objective optimization model and a cut callback procedure is installed.
*	The postsolve step will always be skipped if CPLEX is used to solve a multi-objective optimization model and the model contains a cut pool or filter constraint.


**Learn more about** 

*	:ref:`option-AIMMS-do_postsolve_after_interrupt` 
*	:ref:`option-AIMMS-infeasibility_finder_postsolve` 
*	:ref:`option-AIMMS-mip_calculate_sensitivity_information`  
*	:ref:`option-AIMMS-postsolve_continuous_variables` 
*	:ref:`option-AIMMS-postsolve_integer_variables` 
*	:ref:`option-AIMMS-warning_unreliable_solution` 

