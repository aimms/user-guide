.. _option-CPLEX-deterministic_time_limit:


Deterministic Time Limit
========================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	1e75	



This option sets a time limit expressed in ticks, a unit to measure work done deterministically. 



The length of a deterministic tick may vary by platform. Nevertheless, ticks are normally consistent measures for a given platform (combination of hardware and software) carrying the same load. In other words, the correspondence of ticks to clock time depends on the hardware, software, and the current load of the machine. For the same platform and same load, the ratio of ticks per second stays roughly constant, independent of the model solved. However, for very short optimization runs, the variation of this ratio is typically high. 



CPLEX measures deterministic time only for work inside CPLEX. In other words, deterministic time does not include user algorithms implemented by means of callbacks.



The general solvers option **Time Limit**  sets a time limit measured in seconds.



**Learn more about** 

*	:ref:`option-AIMMS-time_limit`  



