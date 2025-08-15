.. _CONOPT_Limits_-_Limit_Degenerate_Iterations:

Limit on Degenerate Iterations
==============================



:Type:	Integer	
:Range:	{0..:ref:`Miscellaneous_Maxint` }	
:Default:	10	



The default CONOPT pivoting strategy has focus on numerical stability, but it can potentially cycle. When the number of consecutive degenerate iterations exceeds the value of this option, CONOPT will switch to a pivoting strategy that is guaranteed to break degeneracy but with slightly weaker numerical properties.

