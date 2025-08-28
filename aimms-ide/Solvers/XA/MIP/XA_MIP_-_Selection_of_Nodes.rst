.. _option-XA-selection_of_nodes:


Selection of Nodes
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Breadth first	



When solving mixed integer models XA must decide how to handle node generation, as either depth first or breadth first. The depth first approach continues to generate nodes deeper into the branch tree and only backtracks nodes when an infeasibility or integer solution is found. The breadth first approach (the default setting) generates and solves both sides of a node tree before deciding which node to continue with to the next level. This process continues until an infeasibility or integer solution is found.



*	Breadth first
*	Depth first




**Learn more about** 

*	:ref:`option-XA-mip_basis`  



