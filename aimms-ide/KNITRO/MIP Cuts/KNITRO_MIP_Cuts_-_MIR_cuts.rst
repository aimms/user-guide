.. _option-KNITRO-mir_cuts:


MIR Cuts
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies rules for adding mixed integer rounding (MIR) cuts for MINLP problems. Possible values are:



    *	Automatic
    *	None
    *	Root
    *	Tree




With the default setting 'Automatic', let Knitro determine whether to add mixed integer rounding cuts.





With the setting 'None', mixed integer rounding cuts are not added.





With the setting 'Root', add mixed integer rounding cuts derived from equalities at the root node only.





With the setting 'Tree', add mixed integer rounding cuts derived from equalities at every node depending on the solution of the relaxation and the cut generation strategy.

