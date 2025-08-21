.. _option-KNITRO-mip_heuristic_terminate:


MIP Heuristic Terminate
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Feasible	



This option specifies the condition for terminating the MIP heuristic. Possible values are:



*	Feasible
*	Limit




Setting 'Feasible' implies that Knitro terminates at the first feasible point or iteration limit (whichever comes first). Setting 'Limit' means that Knitro will always run to the iteration limit.





**Learn more about** 

*	:ref:`Options_Stop_Criteria_-_Iteration_Limi` 
