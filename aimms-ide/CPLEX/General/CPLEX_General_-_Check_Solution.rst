.. _option-CPLEX-check_solution:


Check Solution
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to check the reliability of the solution. Possible values are:



*	No
*	Yes




If the value of this option equals 'Yes' then the values of the following quantities are calculated:





*   maximum scaled bound infeasibility,
*   maximum unscaled bound infeasibility,
*   number of unscaled bound infeasibilities,
*   maximum unscaled reduced-cost infeasibility,
*   maximum unscaled integer infeasibility (MIP only), and
*   basis condition number ('kappa').




These values are used to check the reliability of the solution. If one of the values is too high, AIMMS generates a warning message.





By default, if the value of this option equals 'Yes' then AIMMS will print statistics that give information about the quality of the solution. This is controlled by the option **Display Solution Statistics** . See the description of that option for more information about the above quantities.





**Note** 

*	This option will only be effective if a solution is found by CPLEX.
*	The basis condition number will not be calculated it the option **Memory Emphasis**  is switched on.
*	In case of a MIP, the basis condition number will only be calculated if the postsolve has been successfully executed. This can be enforced by switching on the general solvers option **MIP Calculate Sensitivity Information** .
*	The solution will not be checked for models with multiple objectives.




**Learn more about** 

*	:ref:`option-CPLEX-display_solution_statistics`  
*	:ref:`option-CPLEX-memory_emphasis`  
*	:ref:`option-AIMMS-mip_calculate_sensitivity_information` 
*	:ref:`option-AIMMS-postsolve` 



