.. _GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts:


Lift and Project Cuts
=====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option determines whether or not to generate lift-and-project cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate lift-and-project cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating lift-and-project cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`  
