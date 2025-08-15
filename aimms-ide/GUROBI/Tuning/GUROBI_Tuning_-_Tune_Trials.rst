.. _GUROBI_Tuning_-_Tune_Trials:


Tune Trials
===========



**Type**:	Integer	

**Range**:	{1 .. 2000000000}	

**Default**:	3



Performance on a MIP model can sometimes experience significant variations due to random effects. As a result, the tuning tool may return option sets that improve on the baseline only due to randomness. This option allows you to perform multiple solves for each option set, using different Seed values for each, in order to reduce the influence of randomness on the results.



**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`GUROBI_Tuning_Tool` 
