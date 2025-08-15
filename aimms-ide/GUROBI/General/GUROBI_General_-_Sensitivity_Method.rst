.. _GUROBI_General_-_Sensitivity_Method:


Sensitivity Method
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which method is used by Gurobi for solving LP problems while calculating sensitivity ranges. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Barrier
*	Opportunistic concurrent
*	Deterministic concurrent




See the option **Method**  for a description of the algorithms.





Multiple LP problems are solved to calculate shadow price ranges for constraints and value ranges for variables. See :ref:`Miscellaneous_Calculation_of_Shadow_Price_Ra`  for more information.





**Note** 

*	The option **Concurrent Method**  controls the methods used by the concurrent solver.




**Learn more about** 

*	:ref:`Options_Sensitivity_-_Calculate_Sensit` 
*	:ref:`GUROBI_General_-_Concurrent_Method` 
*	:ref:`GUROBI_General_-_Method` 



