.. _CONOPT_Stop_Criteria_-_Limit_Slow_Progress:

Limit for Slow Progress
=======================



:Type:	Integer	
:Range:	{2..:ref:`Miscellaneous_Maxint` }	
:Default:	20	



This option sets the maximum number of consecutive iterations of a slow progress. A slow progress means that the optimization is stopped with a "Slow Progress" message if the change in objective is less than **Slow** **Progress Tolerance** * max(1,|fobj|) for the value of this option consecutive iterations, where fobj is the value of the current objective function. 



**Learn more about** 

*	:ref:`CONOPT_Stop_Criteria_-_Slow_Progress_Tol`  



