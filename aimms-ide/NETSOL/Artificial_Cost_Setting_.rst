

.. _Artificial_Cost_Setting_:
.. _NETSOL_Artificial_Cost_Setting_:


Artificial Cost Setting
=======================



**Type** :	Floating point number

**Range** :	[1,inf)	

**Default** :	1.5



For finding an initial feasible solution, NETSOL may introduce some artificial arcs. The cost placed along every artificial arc equals the largest cost in the original network times the value of this option. This cost should be sufficiently large to ensure zero flows along artificial arcs in the initial solution. If this objective is not reached for the current setting of the artificial cost, then the artificial is increased by a factor, which equals the value of the option**Artificial Cost Increase Factor** .



**Learn more about** 


*   :ref:`NETSOL_Artificial_Cost_Increase_Factor`  

