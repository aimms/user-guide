.. _option-Baron-insufficient_progress_termination:


Insufficient progress termination
=================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



Users have the option to request BARON to terminate if insufficient progress is made over δt consecutive seconds where δt is specified by the option **Insufficient Progress Time** .



Progress is measured using the absolute and relative improvement thresholds δa and δr as specified by the options **Absolute Improvement Tolerance**  and **Relative Improvement Tolerance**  respectively.



Termination will occur if, over a period of δt consecutive seconds, the value of the best solution found by BARON is not improved by at least an absolute amount δa or an amount equal to δr times the value of the incumbent at time t−δt.



This termination condition is enforced after processing the root node and only after a feasible solution has been obtained.



Possible values are:



*	Off
*	On




**Learn more about** 

*	:ref:`option-Baron-absolute_improvement_tolerance` 
*	:ref:`option-Baron-insufficient_progress_time` 
*	:ref:`option-Baron-relative_improvement_tolerance` 



