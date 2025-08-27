.. _option-CPLEX-barrier_display:


Barrier Display
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



The setting of this option determines the level of barrier progress information to be displayed. At the default level, no progress information is displayed. At the level "Normal", "normal" setup and iteration information is displayed (see the section "Barrier Input & Output" in Chapter 2 of the CPLEX documentation for a complete interpretation of normal display information). At a setting of "Diagnostics", additional diagnostic information is displayed which may be useful when seeking technical support. Possible values are:



    *	None
    *	Normal
    *	Diagnostics




**Remark** 


The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.





There is no difference between settings 'All' and 'Remark' for option **Solver Listing Messages** , except that with setting 'All' also information is logged for LP problems solved while calculating shadow price ranges for constraints or value ranges for variables, if the barrier algorithm is used to solved those LP problems, as specified by the option **Sensitivity Method** .





**Learn more about** 

*	:ref:`option-CPLEX-sensitivity_method` 
*	:ref:`option-AIMMS-solver_listing`  
*	:ref:`option-AIMMS-solver_listing_messages`  






