.. _GUROBI_Quadratic_-_Nonconvex_Strategy:


Nonconvex Strategy
==================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option specifies the strategy for handling non-convex quadratic programs. Possible values are:



*	Automatic
*	Off
*	Linearize
*	Translate




With setting 'Off', an error is reported if the original user model contains non-convex quadratic constructs. With setting 'Linearize', an error is reported if non-convex quadratic constructs could not be discarded or linearized during presolve. With setting 'Translate', non-convex quadratic problems are solved by means of translating them into a bilinear form and applying spatial branching.





The default setting 'Automatic' is currently almost equivalent to 'Translate', except that it takes less care to avoid presolve reductions that might transform a convex constraint into one that can no longer be detected to be convex, and thus can sometimes perform more presolve reductions.





**Note** 

*	The behavior of the default setting 'Automatic' has changed compared to Gurobi 10.0.
