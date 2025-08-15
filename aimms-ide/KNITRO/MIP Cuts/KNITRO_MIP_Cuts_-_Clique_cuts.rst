.. _KNITRO_MIP_Cuts_-_Clique_cuts:


Clique Cuts
===========

 

**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option specifies rules for adding clique cuts for MINLP problems. Possible values are:



*	Automatic
*	None
*	Root
*	Tree




With the default setting 'Automatic', let Knitro determine whether to add clique cuts. 





With the setting 'None', clique cuts are not added.





With the setting 'Root', add clique cuts derived from equalities at the root node only.





With the setting 'Tree', add clique cuts derived from equalities at every node depending on the solution of the relaxation and the cut generation strategy.







