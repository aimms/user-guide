.. _option-GUROBI-master_knapsack_cuts:


Master Knapsack Cuts
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	


This option controls the generation of cuts derived from the master knapsack polytope. Setting the value different from 'Off' indicates that the
attempt to generate mixing cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness
in generating mixing cuts. Possible values are:

    *	Automatic
    *	Off
    *	Conservative
    *	Aggressive


This option overrides option **Global Cut Control**.


**Note** 

*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-global_cut_control`  
