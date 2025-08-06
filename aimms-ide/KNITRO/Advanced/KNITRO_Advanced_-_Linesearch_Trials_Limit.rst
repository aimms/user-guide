.. _KNITRO_Advanced_-_Linesearch_Trials_Limit:


Linesearch Trials Limit
=======================



**Type** :	Integer	

**Range** :	{1..1000000}	

**Default** :	3	



This option indicates the maximum allowable number of trial points during the linesearch of the Interior-Direct or SQP algorithm before treating the linesearch step as a failure and generating a new step.



This option has no effect on the Interior-CG or Active-Set algorithm.



**Learn more about** 

*	:ref:`KNITRO_Advanced_-_Linesearch_Strategy`  
