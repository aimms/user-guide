

.. _option-AIMMS-constraint_listing_robust_optimization:


Constraint Listing Robust Optimization
======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Robust counterpart	



The robust counterpart for a symbolic mathematical program with uncertain data is generated using the function GMP::Instance::GenerateRobustCounterpart. To do so, AIMMS first collects all symbolic information to generate an intermediate GMP in which all uncertain parameters are treated as variables. This uncertain mathematical program might contain quadratic constraints if uncertain parameters are multiplied by variables, or if the model contains ellipsoidal uncertainty constraints. The generated uncertain mathematical program is then used to construct the robust counterpart GMP.



AIMMS will only print listing files related to robust optimization if the general option **Constraint Listing**  is switched on. Through this specific option **Constraint Listing Robust Optimization**  you can control what listing files are created, if any. If this option is set to 'Uncertain mathematical program' then the constraint listing will be printed for the uncertain mathematical program, and if set to 'Both' then the constraint listing will be printed for the uncertain mathematical program and the robust counterpart GMP. Possible values are:



*	None
*	Uncertain mathematical program
*	Robust counterpart
*	Both




**Note** 

*	If this option is set to 'Uncertain mathematical program' or 'Both' then the memory used by AIMMS might increase significantly.
*	In the constraint listing for the uncertain mathematical program, adjustable variables and variables corresponding to uncertain parameters get a level value of NA because no unique level value exists for them.
*	AIMMS prints the constraint listing(s) if the robust counterpart is solved (e.g., by using the procedure GMP::Instance::Solve) but the constraint listing for the uncertain mathematical program is printed at the beginning of the function GMP::Instance::GenerateRobustCounterpart if the value of the option **Constraint Listing Printed When**  equals 'Before solve' or 'Before and after solve'.




**Learn more about** 

*	:ref:`option-AIMMS-constraint_listing` 
*	:ref:`option-AIMMS-constraint_listing_variable_values`  



