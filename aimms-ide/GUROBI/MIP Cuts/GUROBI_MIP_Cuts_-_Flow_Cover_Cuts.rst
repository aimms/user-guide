.. _option-GUROBI-flow_cover_cuts:


Flow Cover Cuts
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether or not to generate flow cover cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate flow cover cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating flow cover cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`option-GUROBI-global_cut_control`  



