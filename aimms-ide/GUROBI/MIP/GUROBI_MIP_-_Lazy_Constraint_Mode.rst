.. _option-GUROBI-lazy_constraint_mode:

Lazy Constraint Mode
====================

:Type:	Integer	
:Range:	{1 .. 3}	
:Default:	1	

This option determines how a lazy constraint, that is placed in the lazy constraint pool, is handled by Gurobi.

Larger values of this option cause the constraint to be pulled into the model more aggressively. 
With a value of 1, the constraint can be used to cut off a feasible solution, 
but it won't necessarily be pulled in if another lazy constraint also cuts off the solution. 
With a value of 2, all lazy constraints that are violated by a feasible solution will be pulled into the model.
With a value of 3, lazy constraints that cut off the relaxation solution at the root node are also pulled in.

This option sets the mode for all lazy constraints, but the mode can be overwritten for individual rows by using the procedures GMP::Row::SetPoolType and GMP::Row::SetPoolTypeMulti.

**Learn more about** 

*	:any:`GMP::Row::SetPoolType`
*	:any:`GMP::Row::SetPoolTypeMulti`
