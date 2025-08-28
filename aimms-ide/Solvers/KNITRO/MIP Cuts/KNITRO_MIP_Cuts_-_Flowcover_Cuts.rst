.. _option-KNITRO-flow_cover_cuts:


Flow Cover Cuts
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies rules for adding probing cuts for MINLP problems. Possible values are:



    *	Automatic
    *	None
    *	Root
    *	Tree




With the default setting 'Automatic', let Knitro determine whether to add flow cover cuts.





With the setting 'None', flow cover cuts are not added.





With the setting 'Root', add flow cover cuts derived from equalities at the root node only.





With the setting 'Tree', add flow cover cuts derived from equalities at every node depending on the solution of the relaxation and the cut generation strategy.

