.. _option-CPLEX-heuristic_frequency:


Heuristic Frequency
===================



:Type:	Integer	
:Range:	{-1 .. 2147483647}	
:Default:	0	



The value of this option determines how often to apply the periodic heuristic. Setting the value to –1 turns off periodic heuristic. Setting the value to 0, the default, applies the periodic heuristic at an interval chosen automatically. Setting the value to a positive number applies the heuristic at the requested node interval. The heuristics used are somewhat different than the heuristics used with a fixed heuristic frequency.



**Note** 

*	The behavior of CPLEX is undefined if both this option and the option **Heuristic Effort**  are set to non-default values. These two options should not be used together.




**Learn more about** 

*	:ref:`option-CPLEX-heuristic_effort` 
