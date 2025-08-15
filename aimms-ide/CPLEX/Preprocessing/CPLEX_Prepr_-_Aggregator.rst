.. _CPLEX_Prepr_-_Aggregator:


Aggregator
==========



:Type:	Integer	
:Range:	{-1 .. 2100000000}	
:Default:	-1	



This option, when set to a nonzero value, will invoke the CPLEX Aggregator to use substitution where possible to reduce the number of rows and columns before the active problem is solved. If the option is set to a positive value, then the aggregator will be applied the specified number of times, or until no more reductions are possible. At the default value of -1, the aggregator is applied once for LP, and an unlimited number of times for MIP. At this setting, all potential presolve reductions are performed for MIP. Possible values are:



-1:	Default aggregation	

0:	None	

n:	n aggregations		



Another option, which affects only the aggregator, is**Limit Substitutions** . Occasionally the substitutions made by the aggregator will increase matrix density and thus make each iteration too expensive to be advantageous. In such cases, try lowering **Limit Substitutions**  from its default value of 10. CPLEX may make fewer substitutions as a consequence, and the resulting problem will be less dense.



**Learn more about** 

*	 :ref:`CPLEX_Prepr_-_Limit_Substitut` 
