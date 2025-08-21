.. _option-GUROBI-partition_heuristic:

Partition Heuristic
===================

:Type:	Integer	
:Range:	{0 .. 31}	
:Default:	15	

This option controls where the partition heuristic runs. Choices are:

*   Before the root relaxation is solved (16)
*   At the start of the root cut loop (8)
*   At the end of the root cut loop (4)
*   At the nodes of the branch-and-cut search (2)
*   When the branch-and-cut search terminates (1)

The option value is a bit vector, where each bit turns the heuristic on or off at that place. 
The numerical values next to the options listed above indicate which bit controls the corresponding option. 
Thus, for example, to enable the heuristic at the beginning and end of the root cut loop (and nowhere else), 
you would set the 8 bit and the 4 bit to 1, which would correspond to a option value of 12.

The default value of 15 indicates that we enable every option except the first one listed above.

The partitioning heuristic uses large-neighborhood search to try to improve the current incumbent solution. 
To enable the partitioning heuristic a partition should be specified for at least one variable. 
In AIMMS you can specify a partition for a variable using the function GMP::Column::SetDecomposition. 
The provided partition number can be positive, which indicates that the variable should be included when the correspondingly numbered sub-MIP is solved, 0 which indicates that the variable should be included in every sub-MIP, or -1 which indicates that the variable should not be included in any sub-MIP. 
Variables that are not included in the sub-MIP are fixed to their values in the current incumbent solution. If no partition value is assigned to a variable, using the function GMP::Column::SetDecomposition, then its partition value will be -1.

To give an example, imagine you are solving a model with 400 variables and you set the partition attribute to -1 for variables 0-99, 0 for variables 100-199, 1 for variables 200-299, and 2 for variables 300-399. The heuristic would solve two sub-MIP models: sub-MIP 1 would solve for variables 100-199 and 200-299 and fix the other variables (i.e., 0-99 and 300-399) to their values in the incumbent, while sub-MIP 2 would solve for variables 100-199 and 300-399 (and fix variables 0-99 and 200-299).

**Learn more about** 

*	:any:`GMP::Column::SetDecomposition`
