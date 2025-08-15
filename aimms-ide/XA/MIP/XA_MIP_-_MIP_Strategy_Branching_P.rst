.. _XA_MIP_-_MIP_Strategy_Branching_P:


MIP Strategy Branching Priorities
=================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



Each time a node is generated, XA calculates the effect of each non-integer valued integer on future objective function values. This is quite calculation intensive. By assigning branching priorities to the integer variables, XA will only perform this calculation on those non-integer valued integers with the highest branching priority. This often reduces the number of calculations. Setting this option to "Yes" is only effective if priorities to integer variables have been assigned. Possible values are:



*	No
*	Yes




**Remark** 


If you set this option to a non-default value then sometimes the solution time is reduced but XA may not find an optimal integer solution! You should only change the setting of this option if you are interested in obtaining a fast and good integer solution (which may not be optimal).





**Learn more about** 

*	:ref:`XA_MIP_-_MIP_Strategy`  
*	:ref:`XA_MIP_-_MIP_Strategy_Estimate_In`  
*	:ref:`XA_MIP_-_MIP_Strategy_Split_Node_`  



