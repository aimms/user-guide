

.. _option-AIMMS-maximum_number_of_nodes_in_tree:


Maximum Number of Nodes in Tree
===============================



:Type:	Integer	
:Range:	{0 .. 10000000}	
:Default:	1000	



With this option you can determine the maximum number of nodes in the MIP search tree, if the option
**Show Branch and Bound Tree** is active. Note that when the actual solution process requires more
nodes that the specified maximum, the tree displayed on the MIP Search Tree tab on the Math Program
Inspector window will show an incomplete tree.


**Learn more about** 

*	:ref:`Math Program Inspector <aimmshelp26-Math_Program_Inspector>` 
*	:ref:`option-AIMMS-show_branch_and_bound_tree` 

