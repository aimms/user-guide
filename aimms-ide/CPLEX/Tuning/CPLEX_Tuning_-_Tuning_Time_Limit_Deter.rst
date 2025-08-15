.. _CPLEX_Tuning_-_Tuning_Time_Limit_Deter:


Tuning Time Limit Deterministic
===============================



:Type:	Floating point number	
:Range:	[1,inf)	
:Default:	1e75



This option sets a time limit per model and per test set (that is, suite of models) applicable in tuning. 



When this deterministic tuning time limit is set to a finite value, then the tuning finds appropriate settings of other CPLEX options to minimize the deterministic time of optimization, and the tuning process itself is deterministic.



This deterministic time limit on tuning is not compatible with the nondeterministic **Tuning Time Limit**  option (measured in seconds). Only one of these two options can be set to a finite value at a time.



If you want to run a tuning session with unlimited time per model, then set the tuning time limit to a very large value that is smaller than 1e75 (for example, 1e74). When you set the deterministic tuning time limit thus, the tuning process recommends appropriate option setting to minimize deterministic optimization time.



**Learn more about** 

*	:ref:`CPLEX_Tuning_Tool` 
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
*	:ref:`CPLEX_Tuning_-_Tuning_Time_Limit` 
