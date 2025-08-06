.. _CPLEX_Cuts_-_Zero_Half_Cuts:


Zero Half Cuts
==============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines whether or not to zero-half cuts for the problem. Setting the value to "Automatic", the default, indicates that the attempt to zero-half cuts should continue only if it seems to be helping. Possible values are:



*	Off
*	Automatic
*	Generate cuts moderately
*	Generate cuts aggressively




If you find that too much time is spent generating zero-half cuts for your model, consider turning off this option. If the dual bound of your model does not make sufficient progress, consider setting this option to 'Generate cuts aggressively' to generate zero-half cuts more aggressively. 




