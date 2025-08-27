.. _option-KNITRO-barrier_relax_constraints:


Barrier Relax Constraints
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Inequality	



This option indicates whether a relaxation approach is applied to the constraints. Using a relaxation approach may be helpful when the problem has degenerate or difficult constraints. Possible values are:



    *	None
    *	Equality
    *	Inequality
    *	All




With setting 'None' no constraints are relaxed. A relaxation approach is applied to general equality or inequality constraints for settings 'Equality' and 'Inequality' respectively. The last setting implies that a relaxation approach is applied to all general constraints.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
