

.. _Options_Tuning_-_Profiler_Timing_Metho:


Profiler Timing Method
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Performance Count	



This option determines which method is used to calculate the time that is needed to execute a statement. Possible values are:



*	Process Time (The system function clock() is used) 
*	Cpu Cycles (The amount op CPU cycli are counted)
*	Performance Count (Uses QueryPerformanceCount to determine the CPU cycli)
*	Time Slices (Use GetProcessTime to determine the total execution time spent by all threads of the AIMMS process)







Each method has its advantages and disadvantages. 





The advantage of using the Process Time method is that only the time slices that AIMMS uses are measured. The disadvantage is that if multiple statements are executed in 1 timeslice, only the last executed statement will be assigned a time.


The advantages of the Cpu Cycles method is that it has only very small overhead and it is very accurate (when AIMMS is the only process that is taking time). The disadvantages are that other processes are not taken into account, so that some statements might be assigned too much time and it can occur that the amount of Cpu cycli per second are not determined correctly so that all statements are assigned too much or too little time by the same factor.


The advantage of the Performance Count method is that the Cpu Cycles are determined more accurately than with the Cpu Cycles method, but the disadvantage is that the overhead is larger.


The advantage of Time Slices is that it more accurately computes the total cpu time but the overhead is more significant and it is not available on all platforms. It is available on Win32 platforms and if the option is used on a platform on which it is not available the default will be used instead.







