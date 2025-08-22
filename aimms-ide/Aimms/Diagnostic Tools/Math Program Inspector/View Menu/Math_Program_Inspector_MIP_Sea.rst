

.. _Diagnostic-Tools_Math_Program_Inspector_MIP_Sea:


MIP Search Tree
===============

**Description** 

By selecting MIP Search Tree from the View menu, the MIP Search Tree tab is opened. Whenever your linear model is a mixed-integer model, the solver will most probably use a tree search algorithm to solve your problem. During this tree search the algorithm will encounter one or more solutions if the model is integer feasible. Once the search is completed and the optimal solution has been found, you can use the MIP Search Tree tab to view the shape of the search tree and retrieve branching information about the search tree. Currently CPLEX is the only MIP solver in AIMMS that provides this information. The MIP Search Tree is not available if dynamic search is used by CPLEX to solve the MIP model. It is also not available if the MIP model is solved by using the procedure GMP::SolverSession::AsynchronousExecute.



**Improving the search process** 

The size and shape of the search tree might give you some indication that you could use to improve the performance of the solver by tuning one or more solver options. Consider the case in which the search tree algorithm spends a considerable amount of time in parts of the tree that do not seem interesting in retrospect. You might consider to use priorities or another branching rule, in an attempt to direct the search algorithm to a different part of the tree in an earlier stage of the algorithm.



**Controlling search tree memory usage** 

Because all structural and statistical information is kept in memory, displaying the MIP search tree for large MIPs might not be a good idea. Therefore, you are able to control the display (and size) of the search through the options Show_branch_and_bound_progress, Show_branch_and_bound_tree, and Maximum number of nodes in tree.



**Search tree display** 

For every node several solution statistics are available. They are the sequence number, the branch type, the branching variable, the value of the LP relaxation, and the value of the incumbent solution when the node was evaluated. To help you locate the integer solutions in the tree, integer nodes and their parent nodes are displayed in blue.



**Incumbent progress** 

The lower part of the MIP Search Tree tab retrieves all incumbent solutions that have been found during the search algorithm. From this view you are able to conclude for example how much time the algorithm spend before finding the optimal solution, and how much time it took to proof optimality.



**Learn more about** 

*	:ref:`option-AIMMS-show_branch_and_bound_progress`  
*	:ref:`option-AIMMS-show_branch_and_bound_tree` 
*	:ref:`option-AIMMS-maximum_number_of_nodes_in_tree`  






