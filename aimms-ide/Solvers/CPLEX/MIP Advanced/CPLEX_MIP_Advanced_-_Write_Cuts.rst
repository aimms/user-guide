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





By switching on the option **Write Cuts Variable Values**  each cut and constraint that is printed in the constraint list will be followed by a list of variables referenced in that cut or constraint. Such a list contains for each variable its lower bound, its level value and its upper bound. The level values correspond to the fractional solution found at the end of the root node. The lower and upper bounds correspond to the bounds in the presolved model.





**Note** 

*	The presolved model (without cuts) will be printed if this option is set to 'Presolved model plus cuts' and the option **MIP Number of Cut Passes**  is set to -1.




**Learn more about** 

*	:ref:`option-AIMMS-constraint_listing` 
*	:ref:`option-CPLEX-find_fractional_root_solution` 
*	:ref:`option-CPLEX-mip_number_of_cut_passes` 
*	:ref:`option-CPLEX-write_cuts_variable_values` 
