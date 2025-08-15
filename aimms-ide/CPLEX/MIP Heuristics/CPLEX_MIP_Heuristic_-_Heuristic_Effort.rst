.. _CPLEX_MIP_Heuristic_-_Heuristic_Effort:


Heuristic Effort
================



**Type**:	Floating point number	

**Range**:	[0, inf)	

**Default**:	1	



The value of this option is used to increase (if > 1) or decrease (if < 1) the effort that CPLEX spends on heuristics during a MIP solve. If set to 0, no heuristic will run.



**Note** 

*	The behavior of CPLEX is undefined if both this option and the option **Heuristic Frequency**  are set to non-default values. These two options should not be used together.




**Learn more about** 

*	:ref:`CPLEX_MIP_Heuristic_-_Heuristic_Freq` 
