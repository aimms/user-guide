.. _CPLEX_Tuning_-_Tuning_Time_Limit:


Tuning Time Limit
=================



**Type**:	Floating point number	

**Range**:	[1,inf)	

**Default**:	1e75



This option sets a time limit per model and per test set (that is, suite of models) applicable in tuning. 



For an overall time limit on tuning, use the general solvers option **Time Limit** .



**Note** 

*	The option **Tuning Time Limit Deterministic** limits the amount of tuning time spent in deterministic ticks (rather than seconds).




**Learn more about** 

*	:ref:`CPLEX_Tuning_Tool` 
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
*	:ref:`CPLEX_Tuning_-_Tuning_Time_Limit_Deter` 
