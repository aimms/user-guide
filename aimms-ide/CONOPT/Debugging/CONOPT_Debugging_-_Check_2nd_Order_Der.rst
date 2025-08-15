.. _CONOPT_Debugging_-_Check_2nd_Order_Der:

Check 2nd Order Derivatives
===========================



:Type:	Integer	
:Range:	{-1..:ref:`Miscellaneous_Maxint` }		
:Default:	0	



This options controls how often the second order derivatives are tested. Debugging of derivatives is normally only relevant for user-written functions in external equations. Possible values are:




.. list-table::

   * - 0
     - No debugging.
   * - -1
     - The derivatives are tested in the first point in which second derivatives are used only.
   * - +n
     - The derivatives are tested every n-th call.




**Learn more about** 

*	:ref:`CONOPT_Debugging_-_Check_1st_Order_Der` 
*	:ref:`CONOPT_Debugging_-_Tolerance_2nd_Order_Der_Check` 



