

.. _option-AIMMS-show_branch_and_bound_progress:


Show branch and bound progress
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



When using CPLEX to solve a MIP model, use this option to control whether AIMMS should track the progress of the search algorithm by storing all intermediate incumbent solutions that are found during the branch and bound algorithm. This progress is displayed on the MIP Search Tree tab on the Math Program Inspector window. Possible values are:



*	No
*	Yes




**Note** 

*	The MIP Search Tree is not available if dynamic search is used by CPLEX to solve the MIP model.
*	The MIP Search Tree is not available if the MIP model is solved by using the procedure GMP::SolverSession::AsynchronousExecute.




**Learn more about** 

*	:ref:`aimmshelp26-Math_Program_Inspector` 



