.. _option-COPT-memory_limit:


Memory Limit
============



:Type:	Floating point number
:Range:	[0,1e20]
:Default:	1e20



This option can be used to specify a limit on the amount of memory (in MB) that COPT may use while solving the problem. If this limit is reached then COPT will terminate the solve, and AIMMS will report the best solution found so far. By default no memory limit is imposed.



**Note**

*	This option was added in COPT 8.0.
