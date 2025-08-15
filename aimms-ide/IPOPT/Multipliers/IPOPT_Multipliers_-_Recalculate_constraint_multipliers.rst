

.. _IPOPT_Multipliers_-_Recalculate_constraint_multipliers:


Recalculate constraint multipliers
==================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option tells the algorithm to recalculate the equality and inequality multipliers as least square estimates. This asks the algorithm to recompute the multipliers, whenever the current infeasibility is less than the value of the option Recalculate Constraint Multipliers Tolerance. Choosing 'Yes' might be helpful in the quasi-Newton option. However, each recalculation requires an extra factorization of the linear system. If a limited memory quasi-Newton option is chosen, this is used by default.



Possible values are:



*	No (use the Newton step to update the multipliers)
*	Yes (use least-square multiplier estimates)




**Learn more about** 

*	:ref:`IPOPT_Multipliers_-_Recalculate_constraint_multipliers_tolerance` 
