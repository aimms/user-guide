.. _option-CPLEX-qcp_dual_values:


QCP Dual Values
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	If possible	



This option determines whether CPLEX preprocesses a quadratically constrained program (QCP) so that the user can access dual values for the QCP. Possible values are:



*	No
*	If possible
*	Force




If this option is set to 'No', then CPLEX does not calculate dual values for the QCP.





If this option is set to 'If possible', its default value, then CPLEX calculates dual values for the QCP as long as the calculations do not interfere with presolve reductions.





If this option is set to 'Force', then CPLEX calculates dual values and moreover, CPLEX disables any presolve reductions that interfere with these dual-value calculations.




