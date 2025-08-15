.. _CBC_MIP_Cuts_-_Cut_passes_root_node:


Cut passes root node
====================



:Type:	Integer	
:Range:	{-999999 .. 999999}	
:Default:	-1	



This option sets the number of cut passes at root node in the branch-and-cut tree. The default of -1 means that 100 passes are done if the model contains less than 500 columns, 100 passes (but stop if the drop is small) if less than 5000 columns, and 20 otherwise.

