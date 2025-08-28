.. _option-KNITRO-solution_progress_iterations:


Solution Progress Iterations
============================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



The optimization process will terminate if the relative change in the solution estimate is less than the value specified by the option **Solution Progress Tolerance**  for n consecutive iterations, where n is the value of this option.



If set to 0, Knitro chooses this value based on the solver and context. Currently Knitro sets this value to 3 unless the MISQP algorithm (as controlled by the option **MIP Method** ) is being used, in which case the value is set to 1 by default.



**Learn more about** 

*	:ref:`option-KNITRO-mip_method` 
*	:ref:`option-KNITRO-solution_progress_tolerance` 
