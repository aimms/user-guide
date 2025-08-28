.. _option-CONOPT-check_1st_order_derivatives:

Check 1st Order Derivatives
===========================



:Type:	Integer	
:Range:	{-1 .. :ref:`Miscellaneous_Maxint`}		
:Default:	0	



This options controls how often the derivatives are tested. Debugging of derivatives is normally only relevant for user-written functions in external equations. Possible values are:




.. list-table::

   * - 0
     - No debugging.
   * - -1
     - The derivatives are tested in the initial point only.
   * - +n
     - The derivatives are tested in all iterations that can be divided by n, provided the derivatives are computed in this iteration. (During phase 0, 1, and 3 derivatives are only computed when it appears to be necessary.)




**Learn more about** 

*	:ref:`option-CONOPT-check_2nd_order_derivatives`  



