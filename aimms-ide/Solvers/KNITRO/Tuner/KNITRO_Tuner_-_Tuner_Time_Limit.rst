.. _option-KNITRO-tuner_time_limit:


Tuner Time Limit
================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	1e8	



This option specifies, in seconds, the maximum allowable CPU time before terminating the Knitro-Tuner. In contrast, the value of the general solvers option **Time Limit**  places a time limit on each individual Knitro-Tuner solve for a particular option setting. Therefore, the value of this option should be greater than the value for **Time Limit**.



This option only has effect if the option **Tuner**  is switched on.



**Learn more about** 

*	:ref:`option-AIMMS-time_limit`  
*	:ref:`option-KNITRO-tuner`  
