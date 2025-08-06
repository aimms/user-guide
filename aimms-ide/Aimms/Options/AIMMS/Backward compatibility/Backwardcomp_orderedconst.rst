

.. _Options_Backwardcomp_orderedconst:


Ordered Constraint Presentation
===============================



Type:	Selection	

Range:	The settings listed below	

Default:	On	



This option is used to determine the order in which generated constraints are presented. When this options is switched On after generation the constraints are reordered in order to reflect the specification in the Constraints attribute of the Mathematical Program. When this attribute is empty, the order in AllConstraints is used. When this option is switched Off the constraints will be presented in the order of generation. Possible values are:



*	On
*	Off




**Note** 

*	This option setting does not work with the MINOS solver.
