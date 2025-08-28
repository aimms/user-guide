.. _option-KNITRO-tuner_terminate:


Tuner Terminate
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Complete all solves	



This option defines the termination condition for the Knitro-Tuner procedure. Possible values are:



    *	Complete all solves
    *	First locally optimal
    *	First feasible




With setting 'First locally optimal' the tuner will terminate when a run finds a locally optimal solution. With setting 'First Feasible' the tuner will terminate when a run finds a feasible solution.





This option only has effect if the option **Tuner**  is switched on.





**Learn more about** 

*	:ref:`option-KNITRO-tuner`  
