.. _KNITRO_IP_-_Barrier_Refinement:


Barrier Refinement
==================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Off	



This option specifies whether to try to refine the barrier solution for better precision. If enabled, once the optimality conditions are satisfied, Knitro will apply an additional refinement/postsolve phase to try to obtain more precision in the barrier solution. The effect is similar to the effect of enabling the **Crossover Iteration Limit** , but it is usually much more efficient since it does not involve switching to the Active Set algorithm. Possible values are:



*	Off
*	On




This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 
*	:ref:`KNITRO_IP_-_CrossoverIterLimit` 
