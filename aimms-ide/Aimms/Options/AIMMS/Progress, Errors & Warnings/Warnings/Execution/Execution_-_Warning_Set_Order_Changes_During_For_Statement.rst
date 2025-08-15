

.. _Options_Execution_-_Warning_Set_Order_Changes_During_For_Statement:


Warning Set Order Changes During For Statement
==============================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Warning_in_develop_else_off	



If in a For statement you make a change to the order of a set, and that set is the range of any of the current loop indices, the result may not always be what you expect.

This option determines whether you are notified when such an order change occurs.




.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector.
   * - *	Common_warning_default
     - Take action depending on the option 'Common warning default'.
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler.
   * - *	Strict_warning_default
     - Take action depending on the option 'Strict warning default'.
   * - *	Error
     - Issue an error.
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off




The behavior of the For statement has changed a bit since 24.6. AIMMS now determines the next element to iterate based on the element in the previous iteration. 

If the previous element no longer exists or if in the new ordering the next element does not exist, the For statement will terminate the iteration. 



Please note that if you want to change the ordering of set using a For loop, but it is not relevant to iterate according to that ordering, it is recommended to use the Unordered For.





