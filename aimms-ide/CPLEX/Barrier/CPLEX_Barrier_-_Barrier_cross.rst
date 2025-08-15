.. _CPLEX_Barrier_-_Barrier_cross:


Barrier Crossover Algorithm
===========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option determines which, if any, crossover is performed at the end of a barrier optimization. This option also applies when CPLEX uses the barrier algorithm to solve an LP or QP problem, or when it is used to solve the continuous relaxation of an MILP or MIQP at a node in a MIP. Possible values are:



*	Automatic
*	Primal crossover
*	Dual crossover




**Note** 

*	The crossover phase can be switched off by setting the option **Solution Type**  to 'Nonbasic'.




**Learn more about** 

*	:ref:`CPLEX_General_-_Solution_Type` 



