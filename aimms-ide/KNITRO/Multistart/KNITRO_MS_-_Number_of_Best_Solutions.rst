.. _KNITRO_MS_-_Number_of_Best_Solutions:


Number of Best Solutions
========================



**Type**:	Integer	

**Range**:	{0..1000000}	

**Default**:	0	



This option determines the number of best solutions to be found. All solutions will be stored in the solution repository of the mathematical program. At position 1 of that solution repository the best solution is stored, at position 2 the second best solution, and so on. Solutions in the solution repository can be send to the model identifiers by using the AIMMS routine GMP::Solution::SendToModel. For example, with



	GMP::Solution::SendToModel( 'frac1', 2 );



the second best solution for the mathematical program 'frac1' will be send to the model identifiers.



Each point results from a Knitro solve from a different starting point, and must satisfy the absolute and relative feasibility tolerances. Points are distinct if they differ in objective value or some component by the value of option **Solution Distance** .



This option has only effect if the option **Multistart**  is switched on.



**Learn more about** 

*	:any:`GMP::Solution::SendToModel`
*	:ref:`KNITRO_MS_-_Multistart`  
*	:ref:`KNITRO_MS_-_Solution_Distance` 



