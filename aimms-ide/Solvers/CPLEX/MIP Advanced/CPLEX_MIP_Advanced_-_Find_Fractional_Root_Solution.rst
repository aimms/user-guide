.. _option-CPLEX-find_fractional_root_solution:


Find Fractional Root Solution
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This advanced option can be used to assist model developers. **This option should not be enabled in end-user projects!** 



This option decides whether CPLEX should only find, and return, the fractional solution after exploring the root node in the branch-and-bound tree of a MIP solve. Possible values are:



    *	Off
    *	Normal
    *	Always




To improve the formulation of a MIP problem, aiming to reduce the solving time, it often helps to look at the relaxed MIP problem (RMIP) in which all integer variables are relaxed (and therefore are treated as continuous). One step further would be to look at the fractional solution that CPLEX finds after exploring the root node, which has two advantages compared to using a RMIP solution:





*   CPLEX will apply MIP presolving techniques.




*   CPLEX will add cutting planes ("cuts"), resulting in a formulation that is more tight than the RMIP formulation.




Additionally, if this option is activated then you can also choose to print the cuts added by CPLEX at the root node to a file by setting the option **Write Cuts**  to 'Cuts only', or combined with the presolved model if that option is set to 'Presolved model plus cuts'.





Setting 'Normal' is the preferred setting but it does not work for MIP problems for which CPLEX finds an optimal solution at the root node. Setting 'Always' is slower but works also for MIP problems that are solved by CPLEX at the root node.





If this option is activated then CPLEX will interrupt the solve after processing the root node. The fractional solution found will then be passed to AIMMS, which means that the solution passed to AIMMS is not an integer feasible solution! If CPLEX successfully finds a fractional solution at the end of the root node then the program status of the math program will be set to 'Optimal'; the program status will become 'NoSolution' if an error occurred.





**Note** 

*	If this option is activated then CPLEX will use the 'branch-and-cut' algorithm instead of 'dynamic search'. If the option **MIP Search Strategy** is set to 'Apply dynamic search' then this option will be ignored.
*	This option will also be ignored if the option **Use Generic Callbacks**  is switched on, or if a cut callback is installed for the math program in the AIMMS project.
*	Setting the option **Heuristic Effort** to 0 might reduce the time required to finding the fractional root solution.



**Learn more about** 

*	:ref:`option-CPLEX-heuristic_effort` 
*	:ref:`option-CPLEX-mip_search_strategy` 
*	:ref:`option-CPLEX-use_generic_callbacks` 
*	:ref:`option-CPLEX-write_cuts` 
*	:ref:`option-CPLEX-write_cuts_variable_values` 
