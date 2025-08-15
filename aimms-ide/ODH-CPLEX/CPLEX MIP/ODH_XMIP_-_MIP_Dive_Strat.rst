.. _ODH-CPLEX_XMIP_-_MIP_Dive_Strat:


MIP Dive Strategy
=================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



The MIP traversal strategy occasionally performs probing dives, where it looks ahead at both children nodes before deciding which node to choose. The default setting ("Automatic") chooses when to perform a probing dive. CPLEX will never perform probing types if the value is set to "Traditional dive", and it will always perform probing dives if the value is set to "Probing dive". With the setting "Guided dive", the branch direction is guided by the current incumbent, causing the MIP search to spend more time exploring potential solutions that are similar to the current incumbent, consistent with the idea that better solutions can often be found in a small neighborhood of an existing feasible solution. Possible values are:



*	Automatic
*	Traditional dive
*	Probing dive
*	Guided dive



