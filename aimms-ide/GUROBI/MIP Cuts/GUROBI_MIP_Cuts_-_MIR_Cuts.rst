.. _option-GUROBI-mir_cuts:


MIR Cuts
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether or not to generate Mixed Integer Rounding (MIR) cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate MIR cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating MIR cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`option-GUROBI-global_cut_control`  
