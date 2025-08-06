.. _GUROBI_MIP_Cuts_-_Infeasibility_Proof_Cuts:


Infeasibility Proof Cuts
========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines whether or not to generate infeasibility proof cuts for the problem. Setting the value different from 'Off' indicates that the attempt to generate infeasibility proof cuts should be made. Using the default value indicates that Gurobi will determine the appropriate level in aggressiveness in generating infeasibility proof cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




This option overrides option **Global Cut Control** .





**Learn more about** 

*	:ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`  
