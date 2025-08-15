.. _KNITRO_MIP_Cuts_-_Gomory_Cuts:


Gomory Cuts
===========

 

**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option specifies rules for adding Gomory cuts for MINLP problems. Possible values are:



*	Automatic
*	None
*	Root
*	Tree




With the default setting 'Automatic', let Knitro determine whether to add Gomory cuts. 





With the setting 'None', Gomory cuts are not added.





With the setting 'Root', add Gomory cuts derived from equalities at the root node only.





With the setting 'Tree', add Gomory cuts derived from equalities at every node depending on the solution of the relaxation and the cut generation strategy.







