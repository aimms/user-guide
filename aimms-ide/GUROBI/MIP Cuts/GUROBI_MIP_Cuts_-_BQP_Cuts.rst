.. _option-GUROBI-bqp_cuts:


BQP Cuts
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The value of this option determines if there should be an attempt to generate Boolean Quadric Polytope (BQP) cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate BQP cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating BQP cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`option-GUROBI-global_cut_control`  
