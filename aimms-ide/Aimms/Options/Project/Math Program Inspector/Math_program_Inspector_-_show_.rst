

.. _Options_Math_program_Inspector_-_show_:


Show branch and bound progress
==============================



Type:	Selection	

Range:	The settings listed below	

Default:	Yes	



When using CPLEX to solve a MIP model, use this option to control whether AIMMS should track the progress of the search algorithm by storing all intermediate incumbent solutions that are found during the branch and bound algorithm. This progress is displayed on the MIP Search Tree tab on the Math Program Inspector window. Possible values are:



*	No
*	Yes




**Note** 

*	The MIP Search Tree is not available if dynamic search is used by CPLEX to solve the MIP model.
*	The MIP Search Tree is not available if the MIP model is solved by using the procedure GMP::SolverSession::AsynchronousExecute.




**Learn more about** 

*	:ref:`Diagnostic-Tools_AIMMS_Math_Program_Inspector` 



