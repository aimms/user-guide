.. _option-SNOPT-new_superbasics_limit:


New Superbasics Limit
=====================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	99	



This option causes early termination if the number of free variables has increased significantly since the first feasible point. If the number of new superbasics is greater than the value of this option, the nonbasic variables that have not been removed are frozen and the reduced QP is solved to optimality.



