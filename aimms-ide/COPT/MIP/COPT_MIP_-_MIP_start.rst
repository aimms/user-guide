.. _COPT_MIP_-_MIP_start:


MIP Start
=========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



This option determines whether COPT should load a start solution (if available) for solving a MIP model. COPT uses whatever start information is provided to try to construct a complete solution. Possible values are:



*	Off
*	Use full solutions
*	Use partial solutions




Setting 'Use full solutions' means that COPT will only load full and feasible MIP starts.





Setting 'Use partial solutions' means that COPT will only load feasible MIP starts, and complete partial solutions by solving subMIPs.





**Note** 

*	COPT also supports :ref:`COPT_Multiple_MIP_Starts` .




**Learn more about** 

*	:ref:`COPT_MIP_-_MIP_start_node_limit` 
*	:ref:`COPT_Multiple_MIP_Starts` 



