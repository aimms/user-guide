.. _XA_MIP_-_MIP_Strategy_Estimate_In:


MIP Strategy Estimate Integer Solution
======================================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Normal	



This option controls the amount of time spent by XA on estimating the value of a would-be integer solution. The rough-estimate method calculates values that are rough estimates, whereas the fast method spends very little time on calculating estimated integer values. These two methods may eliminate nodes that would have led to better integer solutions. Possible values are:



*	Normal
*	Rough estimate
*	Fast




**Remark** 


If you set this option to a non-default value then sometimes the solution time is reduced but XA may not find an optimal integer solution! You should only change the setting of this option if you are interested in obtaining a fast and good integer solution (which may not be optimal).





**Learn more about** 

*	:ref:`XA_MIP_-_MIP_Strategy`  
*	:ref:`XA_MIP_-_MIP_Strategy_Branching_P`  
*	:ref:`XA_MIP_-_MIP_Strategy_Split_Node_`  



