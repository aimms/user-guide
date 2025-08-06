.. _XA_Advanced_-_Minimal_Absolute_Pi:


Minimal Absolute Pivot Value
============================



**Type** :	Real	

**Range** :	[0,1]	

**Default** :	1e-9	



When selecting a column to leave the basis the column's marginal values that are less than the value of this option (in absolute sense) are rejected. Making pivots with very small values can lead to numeric instability and should be avoided when possible.



**Remark** 

Extreme caution should be exercised when changing the value of this option because of the overall effect on problem feasibility.



**Learn more about** 

*	:ref:`XA_Advanced_-_Maximal_Absolute_Pi`  



