.. _CPLEX_Tuning_-_Tuning_Repeater:


Tuning Repeater
===============

 

**Type** :	Integer	

**Range** :	{1 .. 2100000000}	

**Default** :	1	



This option specifies the number of times tuning is to be repeated on perturbed versions of a given problem. The problem is perturbed automatically by CPLEX permuting its rows and columns. This repetition is helpful when only one problem is being tuned, as repeated perturbation and re-tuning may lead to more robust tuning results. 



This option applies to only one problem in a tuning session. That is, this option is effective only when you are tuning a single problem with the AIMMS routine GMP::Tuning::TuneSingleGMP.



**Note** 

*	If the value of this option is too large then the CPLEX tuning tool might run out of memory.




**Learn more about** 

*	:ref:`CPLEX_Tuning_Tool` 
*	:any:`GMP::Tuning::TuneSingleGMP`
*	:ref:`CPLEX_Tuning_-_Tuning_Measure` 
