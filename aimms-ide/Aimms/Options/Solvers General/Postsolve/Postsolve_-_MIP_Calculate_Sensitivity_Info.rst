

.. _Options_Postsolve_-_MIP_Calculate_Sensitivity_Info:


MIP Calculate Sensitivity Information
=====================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



After solving a MIP problem, sensitivity information (i.e., reduced costs for the variables and shadow prices for the constraints) is not directly available. To get sensitivity information, all integer values have to be fixed and the derived LP problem must be solved. Sensitivity information will not be calculated if the option **Postsolve**  is switched off.



This option controls whether sensitivity information should be calculated. Possible values are:



*	Off
*	Automatic
*	On




At the default setting of 'Automatic', sensitivity information will be calculated if one of the following conditions holds:




*	the property ReducedCost is specified for one of the variables
*	the property ShadowPrice is specified for one of the constraints
*	the option **Always Store Marginals**  is switched on
*	the option **Store Complete Solver Solution**  is switched on




Sensitivity information can also be calculated if lazy constraints are present. The lazy constraints might be present in a pool of lazy constraints or might be added using a lazy constraint callback procedure.





**Note** 

*	Besides sensitivity information, also an optimal basis is calculated.
*	Please check the option **Postsolve**  for more information regarding the postsolve step.
*	If the LP problem solved during the postsolve step appears to be infeasible then no sensitivity information will be available.
*	Sensitivity information will not be calculated in case of multi-objective optimization, even if this option is switched on.
*	If a lazy constraint callback procedure is installed then the postsolve step will only be executed if the option **Postsolve**  is set to 'On'.
*	If a lazy constraint callback procedure is installed then sensitivity information will not be available for the lazy constraints in case either the procedure GMP::SolverSession::Execute or GMP::SolverSession::AsynchronousExecute is used to solve the model.
*	Even if this option is switched on, right-hand-side ranges, shadow price ranges, coefficient ranges and value ranges are not calculated for MIP problems.




**Learn more about** 

*	:ref:`Options_Sensitivity_-_Always_Store_Mar` 
*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`Options_Math_Program_Inspector_-_Store` 



