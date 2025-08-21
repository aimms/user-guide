.. _option-KNITRO-barrier_watchdog:


Barrier Watchdog
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option specifies whether to enable watchdog heuristic for barrier algorithms. In general, enabling the watchdog heuristic makes the barrier algorithms more likely to accept trial points. Specifically, the watchdog heuristic may occasionally accept trial points that increase the merit function, provided that subsequent iterates decrease the merit function. Possible values are:



*	Off
*	On



