.. _KNITRO_MIP_Cuts_-_Zero_Half_cuts:


Zero Half Cuts
==============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option specifies rules for adding zero-half cuts for MINLP problems. Possible values are:



*	Automatic
*	None
*	Root
*	Tree




With the default setting 'Automatic', let Knitro determine whether to add zero-half cuts.





With the setting 'None', zero-half cuts are not added.





With the setting 'Root', add zero-half cuts derived from equalities at the root node only.





With the setting 'Tree', add zero-half cuts derived from equalities at every node depending on the solution of the relaxation and the cut generation strategy.










