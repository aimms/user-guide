.. _CPOPT_General_-_Solution_storage_limit:


Solution storage limit
======================



**Type** :	Integer	

**Range** :	{1..2100000000}	

**Default** :	1	



This option sets the maximum number of feasible solutions found by CP Optimizer that are stored in AIMMS.



If more than one solution is stored then the solutions can be retrieved using GMP functions. For example, assume that x and y are the only variables in the model. Then we can display the values of x and y for each solution as follows:



NrSolutions := GMP::Solution::Count( myGMP );

 

cnt := 1;

while ( cnt <= NrSolutions ) do

  GMP::Solution::SendToModel( myGMP, cnt );

  

  display x, y;

  

  cnt += 1;

endwhile;



where 'myGMP' is an element parameter with range 'AllGeneratedMathematicalPrograms'. See the Function Reference for more information on the functions GMP::Solution::Count and GMP::Solution::SendToModel.



The solution stored at position 1 (in the solution repository) is the final and best solution found by the CP Optimizer. The solutions after the first position are stored with decreasing objective value in case of minimization (and increasing objective value in case of maximization), i.e., the second-best solution is stored as last.



**Note** 

*	The amount of feasible solutions stored will never exceed the value of the option **Solution Limit** .




**Learn more about** 

*	:ref:`CPOPT_General_-_Solution_limit` 
