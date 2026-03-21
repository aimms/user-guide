

.. _option-Baron-number_of_best_solutions:


Number of Best Solutions
========================



:Type:	Integer	
:Range:	{1 .. 2100000000}	
:Default:	1	



This option determines the number of best solutions to be found. All solutions will be stored in the solution repository of the mathematical program. At position 1 of that solution repository the best solution is stored, at position 2 the second best solution, and so on. Solutions in the solution repository can be send to the model identifiers by using the AIMMS routine :any:`GMP::Solution::SendToModel`. For example, with



	GMP::Solution::SendToModel( 'frac1', 2 );



the second best solution for the mathematical program 'frac1' will be send to the model identifiers.



**Learn more about** 

*	:any:`GMP::Solution::SendToModel`
*	:doc:`BARON_General_-_Solutiondistance` 



