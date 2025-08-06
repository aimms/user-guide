.. _PATH_Limits_-_Restart_Limit:


Restart Limit
=============



**Type** :	Integer	

**Range** :	{0 .. 3}	

**Default** :	3	



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

*	:ref:`PATH_Advanced_-_Gradient_Search`  
*	:ref:`PATH_Advanced_-_Initial_Perturb`  
*	:ref:`PATH_Advanced_-_NMS_m-Step_Freq`  
*	:ref:`PATH_Advanced_-_NMS_Initial_Ref`  
*	:ref:`PATH_Advanced_-_NMS_Merit_Funct`  
*	:ref:`PATH_Advanced_-_NMS_Search_Type`  
*	:ref:`PATH_Crash_-_Crash_Method`  
*	:ref:`PATH_Crash_-_Crash_Method_S_Typ`  
*	:ref:`PATH_Crash_-_Max_Nr_Basis_Chang`  



