

.. _option-AIMMS-ordered_constraint_presentation:


Ordered Constraint Presentation
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option is used to determine the order in which generated constraints are presented. When this option
is switched on, the constraints are reordered after generation in order to reflect the specification in the
``Constraints`` attribute of the Mathematical Program. When this attribute is empty, the order in :aimms:set:`AllConstraints`
is used. When this option is switched off, the constraints will be presented in the order of generation. Possible values are:


    *	On
    *	Off


**Note** 

*	This option setting does not work with the :ref:`SolverMINOS` solver.
