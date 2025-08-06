.. _CPLEX_MIP_-_MIP_Emphasis:


MIP Emphasis
============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Balance optimality and feasibility	



This option specifies whether CPLEX should emphasize feasibility or optimality as it solves the problem. Possible values are:



*	Balance optimality and feasibility
*	Emphasize feasibility over optimality
*	Emphasize optimality over feasibility
*	Emphasize moving best bound
*	Emphasize hidden feasibility
*	Emphasize heuristics




With the default setting of "Balance optimality and feasibility", CPLEX works toward a rapid proof of an optimal solution, but balances that with effort toward finding high quality feasible solutions early in the optimization. 





If the value is set to "Emphasize feasibility over optimality", CPLEX uses tactics designed to find the first and subsequent feasible solutions more quickly, at the likely expense of prolonging the time required to find a proven optimal solution.





When set to "Emphasize optimality over feasibility", less effort may be applied to finding feasible solutions early.





With the setting "Emphasize moving best bound," even greater emphasis is placed on proving optimality through moving the best bound value, so that the detection of feasible solutions along the way becomes almost incidental.





If the value is set to "Emphasize hidden feasibility", the MIP optimizer works hard to find high quality feasible solutions that are otherwise very difficult to find. You should use this setting when you are more interested in a good feasible solution than a provably optimal solution, and when feasibility emphasis has difficulty finding solutions of acceptable quality.





When this option is set to "Emphasize heuristics", the MIP optimizer entirely focuses on finding high quality heuristic solutions as early as possible, and puts almost no effort in moving the best bound and proving optimality. This setting should be considered when the proof of optimality is either not important or is out of reach, and the other settings have difficulty finding solutions of acceptable quality.




