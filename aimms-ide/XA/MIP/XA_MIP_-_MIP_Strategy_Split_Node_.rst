.. _XA_MIP_-_MIP_Strategy_Split_Node_:


MIP Strategy Split Node List
============================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No splitting	



Normally XA does not split up the node list during the branch and bound search process. This option can be used to reduce the number of nodes to evaluate by splitting up the node list. The setting "split list in half" splits the node list in half based on the current length of the list. The setting "split list based on objective value" splits the list based upon the difference between the current projected objective and the best possible objective value divided by two. Using one of these methods will allow XA to search nodes that might normally not be explored. However, the reported integer solution may not be optimal, because nodes that would lead to the optimal solution may be eliminated. Possible values are:



*	No splitting
*	Split list in half
*	Split list based on objective value




**Remark** 


If you set this option to a non-default value then sometimes the solution time is reduced but XA may not find an optimal integer solution! You should only change the setting of this option if you are interested in obtaining a fast and good integer solution (which may not be optimal).





**Learn more about** 

*	:ref:`XA_MIP_-_MIP_Strategy`  
*	:ref:`XA_MIP_-_MIP_Strategy_Branching_P`  
*	:ref:`XA_MIP_-_MIP_Strategy_Estimate_In`  



