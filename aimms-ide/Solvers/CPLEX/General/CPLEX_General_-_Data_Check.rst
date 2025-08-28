.. _option-CPLEX-data_check_and_modeling_assistance:


Data Check and Modeling Assistance
==================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option decides whether data should be checked for consistency and whether CPLEX should offer modeling assistance. Possible values of this option are:



    *	Off
    *	Warn
    *	Assist




When this option is set to 'Warn', CPLEX performs an extensive checking of data as passed to CPLEX, such as checking that indices are within range, that there are no duplicate entries, and that values are valid for the type of data or are valid numbers. This checking is useful for debugging applications.





When the value of this option is set to 'Assist', CPLEX turns on both data consistency checking and modeling assistance. At this level, CPLEX issues warnings at the start of the optimization about coefficients, bounds, and right-hand-side values (RHS) that are inappropriately large or small (in absolute sense). With this setting, when CPLEX solves a model then CPLEX examines features of the model that can impede performance or produce numerical instability (even if the features are otherwise valid). When CPLEX detects such detrimental or unstable features as it solves your model, it issues a warning and suggests possible improvements. For example, the following warnings are typical of such situations:





CPLEX Warning 1040: Detected a big coefficient for a binary


variable in a constraint. In constraint c171832, variable


x490416 has a coefficient 1000.21 times larger than second


largest. Consider turning constraint into an indicator.





CPLEX Warning 1041: Detected big-M constraint that could be


turned into an indicator. In constraint c8095, variable x354


has a bigM of 1000 and could be turned into indicator.





CPLEX Warning 1042: Detected a variable bound constraint with


large coefficients. Constraint c8101, links binary variable


x934 with variable x2642 and the ratio between the two is


1e+06. Consider turning constraint into an indicator for


better performance and numerical stability.





These message are printed in the Messages Window, and the CPLEX log file (if enabled).

