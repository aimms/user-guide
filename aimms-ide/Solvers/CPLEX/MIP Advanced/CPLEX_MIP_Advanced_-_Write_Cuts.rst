.. _option-CPLEX-write_cuts:


Write Cuts
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option can be used to print the cutting planes ("cuts") that CPLEX added while processing the root node in the branch-and-bound tree of a MIP solve. Possible values are:



    *	Off
    *	Cuts only
    *	Presolved model plus cuts




With setting 'Presolved model plus cuts' the presolved model will be printed as well. Information on the cuts and presolved model can be useful if you want to improve the formulation of a MIP problem, aiming to reduce the solving time.





This option can only be used in combination with the option **Find Fractional Root Solution**.





The cuts and presolved model will be written to the file 'cplex_cuts.lis' which will be placed in the log directory of the AIMMS project. It uses a style similar to the constraint listing, which can be printed by AIMMS by using the Solvers General option **Constraint Listing**.





By switching on the option **Write Cuts Variable Values** each cut and constraint that is printed in the constraint list will be followed by a list of variables referenced in that cut or constraint. Such a list contains for each variable its lower bound, its level value and its upper bound. The level values correspond to the fractional solution found at the end of the root node. The lower and upper bounds correspond to the bounds in the presolved model.





**Note** 

*	The presolved model (without cuts) will be printed if this option is set to 'Presolved model plus cuts' and the option **MIP Number of Cut Passes** is set to -1.
*	Setting the option **Heuristic Effort** to 0 might reduce the time required to write the cuts.



**Learn more about** 

*	:doc:`Constraints_-_Constraint_Listi <../../../Aimms/Options/Solvers General/Standard Reports/Constraints/Constraints_-_Constraint_Listi>` 
*	:doc:`CPLEX_MIP_Advanced_-_Find_Fractional_Root_Solution <CPLEX_MIP_Advanced_-_Find_Fractional_Root_Solution>` 
*	:doc:`CPLEX_MIP_Heuristic_-_Heuristic_Effort <../MIP Heuristics/CPLEX_MIP_Heuristic_-_Heuristic_Effort>` 
*	:doc:`CPLEX_Cuts_-_MIP_Nr_of_Cut_Pa <../MIP Cuts/CPLEX_Cuts_-_MIP_Nr_of_Cut_Pa>` 
*	:doc:`CPLEX_MIP_Advanced_-_Write_Cuts_Variable_Val <CPLEX_MIP_Advanced_-_Write_Cuts_Variable_Val>` 
