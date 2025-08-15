

.. _Options_Math_program_inspector_-_feas_tol:


MPI feasibility tolerance
=========================



**Type**:	Selection	

**Range**:	[0,1]	

**Default**:	0.0001	



When determining a substructure causing infeasibility, the Math Program Inspector will add slack variables to variable bounds and to constraints. All variables and constraints whose slack variables exceed the 'feasibility tolerance' will be marked as contributing to the infeasibility. For badly scaled models, it might be necessary to decrease the value of this option.



In addition, the 'feasibility tolerance' is used to determine statistics presented by the Math Program Inspector. More specific, the 'feasibility tolerance' is used to determine whether or not

*	a constraint is infeasibile, and
*	a variable is infeasible (wrt its bounds)




**Note** 

*	For badly scaled models, a discrepancy between the results from the solver and the statistics reported by the Math Program Inspector might occur for some values of the 'feasibility tolerance' (and/or 'bound tolerance').
*	This tolerance is not used for calculating the maximum and total constraint violation on the Constraint Statistics tab.




**Learn more about** 

*	:ref:`Diagnostic-Tools_AIMMS_Math_Program_Inspector` 









