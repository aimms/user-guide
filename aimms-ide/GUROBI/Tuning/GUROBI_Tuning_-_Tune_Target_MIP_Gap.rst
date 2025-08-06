.. _GUROBI_Tuning_-_Tune_Target_MIP_Gap:


Tune Target MIP Gap
===================



**Type** :	Floating point number	

**Range** :	[0,1e100]	

**Default** :	0.005



This option sets a target MIP gap to be reached. As soon as the tuner has found option settings that allow Gurobi to reach the target MIP gap for the given model(s), it stops trying to improve option settings further. Instead, the tuner switches into the cleanup phase (see the **Tune Cleanup**  option).



**Learn more about** 

*	:ref:`GUROBI_Tuning_-_Tune_Cleanup` 
*	:ref:`GUROBI_Tuning_Tool` 
