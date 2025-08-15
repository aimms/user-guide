.. _SNOPT_Advanced_-_Expand_Frequency:


Expand Frequency
================



**Type**:	Integer	

**Range**:	{0..1000000}	

**Default**:	10000	



This option is part of the anti-cycling procedure designed to make progress even on highly degenerate problems. For linear models, the strategy is to force a positive step at every iteration, at the expense of violating the bounds on the variables by a small amount. Suppose that the value of this option is denoted by i and the **Feasibility Tolerance**  by f. Over a period of i iterations, the tolerance actually used by SNOPT increases from 0.5f to f (in steps of 0.5f/i).



For nonlinear models, the same procedure is used for iterations in which there is only one superbasic variable. (Cycling can occur only when the current solution is at a vertex of the feasible region.) Thus, zero steps are allowed if there is more than one superbasic variable, but otherwise positive steps are enforced.

Increasing the value of this option helps to reduce the number of slightly infeasible nonbasic basic variables (most of which are eliminated during a resetting procedure). However, it also diminishes the freedom to choose a large pivot element (see **Pivot Tolerance** ).



**Learn more about** 

*	:ref:`SNOPT_Feasibility_-_Feasibility_Tole`  
*	:ref:`SNOPT_Advanced_-_Pivot_Tolerance`  



