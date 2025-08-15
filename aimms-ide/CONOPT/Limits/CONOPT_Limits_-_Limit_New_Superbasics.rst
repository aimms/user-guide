.. _CONOPT_Limits_-_Limit_New_Superbasics:

Limit on New Superbasics
========================



:Type:	Integer	
:Range:	{0..:ref:`Miscellaneous_Maxint` }	
:Default:	0	



When there has been a sufficient reduction in the reduced gradient in one subspace new non-basics can be selected to enter the superbasis. The ones with largest reduced gradient of proper sign are selected, up to a limit.



If the value of this option is positive then the limit is min(500,value).



If the value of this option is 0 (the default) then the limit is selected dynamically by CONOPT depending on model characteristics.

