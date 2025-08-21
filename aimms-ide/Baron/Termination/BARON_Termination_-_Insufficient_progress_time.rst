.. _option-Baron-insufficient_progress_time:


Insufficient progress time
==========================



:Type:	Floating point number	
:Range:	[-1e51,1e51]	
:Default:	-100	



If the option Insufficient Progress Termination is switched on, BARON will terminate if insufficient progress is made over δt consecutive seconds where δt denotes the value of this option.



If δt is set to a non-positive quantity, BARON will automatically set δt equal to −δt times the CPU time taken till the end of root node processing.



**Learn more about** 

*	:ref:`option-Baron-absolute_improvement_tolerance` 
*	:ref:`option-Baron-insufficient_progress_termination` 
*	:ref:`option-Baron-relative_improvement_tolerance` 



