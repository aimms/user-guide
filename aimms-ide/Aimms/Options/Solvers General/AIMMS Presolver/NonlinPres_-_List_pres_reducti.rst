

.. _option-AIMMS-list_presolve_reductions:


List Presolve Reductions
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



This option controls the frequency with which the reductions by the AIMMS Presolver are printed in the listing file. Possible values are:



    *	Never
    *	At first solve
    *	At an infeasible solve
    *	At every solve




The reductions that are printed to the listing file are the upper and lower bounds of the variables that are tightened by the AIMMS Presolver, and the constraints and variables that are deleted.





If the option **MINLP Probing**  is switched on then also the nonlinear constraints that have been linearized are reported.





**Note** 

*	The options **Solution Listing Column Name Style**  and **Solution Listing Row Name Style**  control the style used for referencing the variables and constraints when printing the presolve reductions.




**Learn more about** 

*	:ref:`option-AIMMS-minlp_probing` 
*	:ref:`option-AIMMS-scale_model` 
*	:ref:`option-AIMMS-solution_listing_column_name_style` 
*	:ref:`option-AIMMS-solution_listing_row_name_style` 
