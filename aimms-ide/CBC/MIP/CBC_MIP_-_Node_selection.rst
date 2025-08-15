.. _CBC_MIP_-_Node_selection:


Node selection
==============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Fewest infeasibilities	



This option determines what strategy to use to select nodes. Possible values are:



*	Hybrid
*	Fewest infeasibilities
*	Depth first
*	Up branch fewest infeasibilities
*	Down branch fewest infeasibilities
*	Up branch depth first
*	Down branch depth first




Normally before a solution CBC will choose the node with fewest infeasibilities. You can choose depth as the criterion. You can also say if up or down branch must be done first (the up down choice will carry on after solution). Setting 'hybrid' means breadth first on small depth nodes then fewest.

