

.. _Miscellaneous_Calculation_of_Shadow_Price_Ra:


Calculation of Shadow Price Ranges
==================================

**Description** 

For an LP problem




.. list-table::

   * -  (P) 
     - MAX
     - c^T x
   * - 
     - s.t. 
     - Ax ≤ b
   * - 
     - 
     - x ≥ 0




AIMMS can calculate the shadow price ranges. The dual problem is given by




.. list-table::

   * -  (D) 
     - MIN
     - b^T y
   * - 
     - s.t. 
     - A^T y ≥ c
   * - 
     - 
     - y ≥ 0




The shadow price range for constraint i is calculated by solving the following two problems




.. list-table::

   * -  (S_max_i) 
     - MAX
     - y_i
   * - 
     - s.t. 
     - A^T y ≥ c
   * - 
     - 
     - b^T y = D_obj
   * - 
     - 
     - y ≥ 0




and




.. list-table::

   * -  (S_min_i) 
     - MIN
     - y_i
   * - 
     - s.t. 
     - A^T y ≥ c
   * - 
     - 
     - b^T y = D_obj
   * - 
     - 
     - y ≥ 0




where D_obj denotes the optimal solution value of (D). The optimal solution value of (S_max_i) gives the largest shadow price and (S_min_i) the smallest shadow price.



In practice the problems (S_max_i) and (S_min_i) are sometimes infeasible because of numerical problems with the constraint



	b^T y = D_obj .



Therefore AIMMS uses the constraint



	b^T y ≤ R



instead where R is defined as



 	MAX[ D_obj * (1.0 +-eps_rel), D_obj + eps_abs ]	if D_obj ≥ 0.0

 	MAX[ D_obj * (1.0 -+eps_rel), D_obj + eps_abs ]	if D_obj ≤ 0.0



Here eps_rel is the value of the option **Shadow Price Range Relative Tolerance**  and eps_abs the value of **Shadow Price Range Absolute Tolerance** . When the setting of both options is 0.0 (the default) R equals D_obj.



**Remark** 

The subproblems (S_max_i) and (S_min_i) are not solved for constraints for which the nominal right hand side value is in the interior of the interval



	[smallest right hand side, largest right hand side]



since for these constraints it is known that



	smallest shadow price = largest shadow price = shadow price.



(Calculating the smallest and largest right hand side values is only supported by CPLEX and Gurobi, so only these solvers can skip solving some of the subproblems (S_max_i) and (S_min_i).)



**Note** 

*	The option **Time Limit Sensitivity Ranges**  can be used to set a time limit for each LP problem that is solved while calculating shadow price ranges (or variable value ranges).




**Learn more about** 

*	:ref:`option-AIMMS-shadow_price_range_absolute_tolerance`  
*	:ref:`option-AIMMS-shadow_price_range_relative_tolerance` 
*	:ref:`option-AIMMS-time_limit_sensitivity_ranges`  



