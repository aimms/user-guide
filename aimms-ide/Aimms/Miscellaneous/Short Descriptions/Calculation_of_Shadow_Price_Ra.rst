

.. _Miscellaneous_Calculation_of_Shadow_Price_Ra:


Calculation of Shadow Price Ranges
==================================

**Description** 

AIMMS can calculate the shadow price ranges for an LP problem:

.. math::

   \begin{aligned}
   \text{(P)} \qquad & \text{Max} \quad && c^Tx \\
   & \text{s.t.} \quad && Ax \leq b \\
   & && x \geq 0
   \end{aligned}


The dual problem is given by

.. math::

   \begin{aligned}
   \text{(D)} \qquad & \text{Min} \quad && b^Ty \\
   & \text{s.t.} \quad && A^Ty \geq c \\
   & && y \geq 0
   \end{aligned}


The shadow price range for constraint :math:`i` is calculated by solving the following two problems

.. math::

   \begin{aligned}
   \text{(Smax)} \qquad & \text{Max} \quad && y_i \\
   & \text{s.t.} \quad && A^Ty \geq c \\
   & && b^Ty = D_{obj} \\
   & && y \geq 0
   \end{aligned}

and

.. math::

   \begin{aligned}
   \text{(Smin)} \qquad & \text{Min} \quad && y_i \\
   & \text{s.t.} \quad && A^Ty \geq c \\
   & && b^Ty = D_{obj} \\
   & && y \geq 0
   \end{aligned}


where :math:`D_{obj}` denotes the optimal objective value of (D). The optimal objective value of (Smax) gives the largest
shadow price and that of (Smin) the smallest shadow price for constraint :math:`i`.

In practice the problems (Smax) and (Smin) are sometimes infeasible because of numerical problems with the constraint

.. math::

   b^Ty = D_{obj}


Therefore AIMMS uses the constraint

.. math::

   b^Ty \leq R


instead where :math:`R` is defined as

.. math::

    R = \begin{cases}
    \text{max}[ D_{obj} * (1 + \epsilon_r), D_{obj} + \epsilon_a ]  \quad  \text{if } D_{obj} \geq 0.0 \\
    \text{max}[ D_{obj} * (1 - \epsilon_r), D_{obj} + \epsilon_a ]  \quad  \text{if } D_{obj} \leq 0.0
    \end{cases}

Here :math:`\epsilon_r` is the value of the option **Shadow Price Range Relative Tolerance** and
:math:`\epsilon_a` the value of the option **Shadow Price Range Absolute Tolerance**. Note that if both
options are set to 0 (the default) then :math:`R = D_{obj}`, otherwise :math:`R > D_{obj}`.


**Remark** 

The subproblems (Smax) and (Smin) are not solved for constraints for which the nominal right-hand- side
value is in the interior of the interval


	[smallest right-hand-side, largest right-hand-side]


since for these constraints it is known that


	smallest shadow price = largest shadow price = shadow price.


Calculating the smallest and largest right-hand-side values is only supported by CPLEX and Gurobi,
so only these solvers can skip solving some of the subproblems (Smax) and (Smin).


**Note** 

*	The option **Time Limit Sensitivity Ranges** can be used to set a time limit for each LP problem that is solved while calculating shadow price ranges (or variable value ranges).




**Learn more about** 

*	:ref:`option-AIMMS-shadow_price_range_absolute_tolerance`  
*	:ref:`option-AIMMS-shadow_price_range_relative_tolerance` 
*	:ref:`option-AIMMS-time_limit_sensitivity_ranges`  



