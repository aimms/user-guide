.. _option-KNITRO-node_selection:


Node Selection
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies the MIP selection rule for choosing the next node in the branch and bound tree. Possible values are:



*	Automatic
*	Depth first
*	Best bound
*	Combo 1




Setting 'Best bound' implies selecting the node with the best relaxation bound. Setting 'Combo 1' means use depth first unless pruned, then best bound.




