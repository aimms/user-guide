.. _GUROBI_Quadratic_-_NLP_Heuristic:


NLP Heuristic
=============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Yes	



This option determines whether Gurobi should use an NLP heuristic to find feasible solutions to non-convex quadratic models. Possible values are:



*	No
*	Yes




The NLP heuristic uses a non-linear barrier solver to find feasible solutions to non-convex quadratic models. It can often find solutions much more quickly than the alternative, but in some cases it can consume significant runtime without producing a solution. 





**Note** 

*	This option only affects non-convex quadratic models.




**Learn more about** 

*	:ref:`GUROBI_Quadratic_-_Nonconvex_Strategy` 
