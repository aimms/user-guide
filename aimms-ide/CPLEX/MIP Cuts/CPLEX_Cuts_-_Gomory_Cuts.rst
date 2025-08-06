.. _CPLEX_Cuts_-_Gomory_Cuts:


Gomory Cuts
===========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines whether or not to generate Gomory (fractional) cuts for the problem. Setting the value to "Automatic", the default, indicates that the attempt to generate Gomory cuts should continue only if it seems to be helping. Possible values are:



*	Off
*	Automatic
*	Generate cuts moderately
*	Generate cuts aggressively




**Note** 

*	This option can also be used for MIQP problems. For MIQP problems the default setting 'Automatic' means that no Gomory cuts will be generated.



