.. _option-ODHCPLEX-number_of_iterations_in_presolve:


Number of Iterations in Presolve
================================



:Type:	Integer	
:Range:	{-1 .. 2100000000}	
:Default:	-1	



The setting of this option determines the number of presolve iterations made. When set to a non-zero value, CPLEX will invoke presolve to simplify and reduce problems. When set to a positive value, the presolve will be applied the specified number of times, or until no more reductions are possible. At the default value of –1, Presolve should continue only if it seems to be helping.



