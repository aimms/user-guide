.. _option-KNITRO-initial_point_strategy:


Initial Point Strategy
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether or not the interior-point algorithms in Knitro should shift the given initial point (before starting the optimization) to satisfy bounds on the variables. If the options **Honor Bounds**  or **Feasible Mode**  are enabled, then a request to shift may be ignored. At the default value Knitro decides. Possible values are:



    *	Automatic
    *	Strategy 1
    *	Strategy 2
    *	Strategy 3




**Learn more about** 

*	:ref:`option-KNITRO-feasible_mode`  
*	:ref:`option-KNITRO-honor_bounds`  
