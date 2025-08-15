.. _GUROBI_MIP_Cuts_-_Clique_Cuts:


Clique Cuts
===========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



The value of this option determines if there should be any attempt to generate clique cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate clique cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating clique cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`  
