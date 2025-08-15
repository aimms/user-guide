

.. _IPOPT_Line_search_-_Watchdog_shortened_iteration_trigger:


Watchdog shortened iteration trigger
====================================



:Type:	Integer	
:Range:	{0..2147483647}	
:Default:	10	



This option set the number of shortened iterations that trigger the watchdog. If the number of successive iterations in which the backtracking line search did not accept the first trial point exceeds this number, the watchdog procedure is activated. Choosing 0 disables the watchdog procedure.

