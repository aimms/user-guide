

.. _option-AIMMS-show_branch_and_bound_tree:


Show Branch and Bound Tree
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



When using :ref:`SolverCPLEX` to solve a MIP model, AIMMS is able to register the size and shape of the search tree used
during the MIP. This tree can be viewed on the MIP Search Tree tab of the Math Program Inspector window after the model
has been solved. Storing tree information may require a lot of memory. Therefore, by default, no tree information will be
stored. Possible values are:

    *	No
    *	Yes


The number of nodes shown in the MIP Search Tree is limited by the option **Maximum Number of Nodes in Tree**.


**Note** 

*	The MIP Search Tree is only available for CPLEX if the CPLEX option **MIP Search Strategy** is set to 'Apply branch-and-cut'.
*	The MIP Search Tree is not available if parallel CPLEX is used.
*	The MIP Search Tree is not available if the MIP model is solved by using the procedure :any:`GMP::SolverSession::AsynchronousExecute`.
*	If this option is switched on then the CPLEX option **MIP Display** will be temporarily set to 'Display each nth node' if that option was set to 'None' (the default), 'Display integer feasible solutions' or 'Nth node + LP display for all nodes'.
*	If this option is switched on then the CPLEX option **MIP Interval** will be temporarily set to 1.


**Learn more about** 

*	:ref:`Math Program Inspector <aimmshelp26-Math_Program_Inspector>` 
*	:ref:`option-AIMMS-maximum_number_of_nodes_in_tree` 
*	:ref:`option-CPLEX-mip_search_strategy` 
*	:ref:`option-CPLEX-mip_display` 
*	:ref:`option-CPLEX-mip_interval` 

