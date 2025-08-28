.. _option-PATH-restart_limit:


Restart Limit
=============



:Type:	Integer	
:Range:	{0 .. 3}	
:Default:	3	



This option sets the maximal number of restarts that PATH should make if it could not find a feasible solution. PATH first tries to find a feasible solution with the current settings of the options. If PATH fails it restarts the solving process by using different kind of option settings. The option settings corresponding to the restart numbers are given in the following table, where "residual" denotes a measure of how far the initial point (given to PATH) is from satisfying the complementarity conditions.






.. list-table::

   * - **Restart number** 
     - **Option name** 
     - **Option value** 
   * - 1
     - Initial Perturbation
     - 0.01 * residual
   * - 
     - NMS Initial Reference Factor
     - 2.0
   * - 
     - Crash Method
     - None
   * - 2
     - Initial Perturbation
     - 0.0
   * - 
     - NMS m-Step Frequency
     - 1
   * - 
     - NMS Initial Reference Factor
     - 10.0
   * - 
     - NMS Merit Function Values Storage
     - 2
   * - 
     - Crash Method
     - None
   * - 3
     - Gradient Search Type
     - Arc
   * - 
     - Initial Perturbation
     - 0.0
   * - 
     - NMS Initial Reference Factor
     - 2.0
   * - 
     - NMS Search Type
     - Arc
   * - 
     - Crash Method
     - Pnewton
   * - 
     - Crash Method Search Type
     - Arc
   * - 
     - Maximal Number of Basis Changes
     - 10
   * - 
     - 
     - 




**Learn more about** 

*	:ref:`option-PATH-gradient_search_type`  
*	:ref:`option-PATH-initial_perturbation`  
*	:ref:`option-PATH-nms_m-step_frequency`  
*	:ref:`option-PATH-nms_initial_reference_factor`  
*	:ref:`option-PATH-nms_merit_function_values_storage`  
*	:ref:`option-PATH-nms_search_type`  
*	:ref:`option-PATH-crash_method`  
*	:ref:`option-PATH-crash_method_search_type`  
*	:ref:`option-PATH-maximal_number_of_basis_changes`  



