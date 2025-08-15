.. _GUROBI_MIP_Cuts_-_Flow_Path_Cuts:


Flow Path Cuts
==============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option determines whether or not to generate flow path cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate flow path cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating flow path cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`  
