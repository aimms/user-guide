

.. _option-AIMMS-show_branch_and_bound_progress:


Show Branch and Bound Progress
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



When using :ref:`SolverCPLEX`, :ref:`SolverGurobi` or :ref:`SolverCOPT` to solve a MIP model, use this option to control whether
AIMMS should track the progress of the search algorithm by storing all intermediate incumbent solutions that are found during
the branch and bound algorithm. This progress is displayed on the MIP Search Tree tab on the Math Program Inspector window.
Possible values are:

    *	No
    *	Yes


**Note** 

*	The MIP Search Tree is only available for CPLEX if the CPLEX option **MIP Search Strategy** is set to 'Apply branch-and-cut'.
*	The MIP Search Tree is not available if the MIP model is solved by using the procedure :any:`GMP::SolverSession::AsynchronousExecute`.


**Learn more about** 

*	:ref:`Math Program Inspector <aimmshelp26-Math_Program_Inspector>` 
*	:ref:`option-CPLEX-mip_search_strategy` 

