

.. _option-AIMMS-suppress_listing_file_encrypted_project:


Suppress Listing File Encrypted Project
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option controls whether or not writing of the constraint and solution listing or the irreducible infeasibility set (IIS) should be suppressed for encrypted AIMMS projects (.aimmspack files). Possible values are:



    *	On
    *	Off




By default AIMMS will suppress the writing of the constraint and solution listing and the IIS for encrypted AIMMS projects. The constraint and solution listing are controlled by the options **Constraint Listing**  and **Solution Listing**  respectively. Printing of the IIS is controlled by the option **Infeasibility Finder** .





**Note** 

*	You should switch off this option if you want to print the constraint or solution listing or IIS in an end-user project (because end-user projects are always encrypted).
*	This option also influences the option **Solver Column Row Mapping** .




**Learn more about** 

*	:ref:`option-AIMMS-constraint_listing` 
*	:ref:`option-AIMMS-infeasibility_finder` 
*	:ref:`option-AIMMS-solution_listing` 
*	:ref:`option-AIMMS-solver_column_row_mapping` 



