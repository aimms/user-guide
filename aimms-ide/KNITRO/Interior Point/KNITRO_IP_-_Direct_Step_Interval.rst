.. _KNITRO_IP_-_Direct_Step_Interval:


Direct Step Interval
====================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	10	



This option controls the maximum number of consecutive conjugate gradient (CG) steps before Knitro will try to enforce that a step is taken using direct linear algebra. This option is only valid for the Interior/Direct algorithm and may be useful on problems where Knitro appears to be taking lots of conjugate gradient steps.



Setting the value to 0 will try to enforce that only direct steps are taken which may produce better results on some problems.



**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 



