.. _option-GUROBI-relax-and-lift_cuts:


Relax-and-Lift Cuts
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The value of this option determines if there should be an attempt to generate relax-and-lift cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate relax-and-lift cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating relax-and-lift cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`option-GUROBI-global_cut_control` 
