.. _option-ODHCPLEX-recurse_iteration_limit_solution:


Recurse Iteration Limit Solution
================================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	2100000000	



This option specifies the iteration limit for the recurse heuristic for sub-solves in case a solution is found by the recurse heuristic. Please note that with default settings the recurse heuristic, even if it finds a solution, will stop after it hits the **Recurse Iteration Limit**. That is, with default settings this option is inactive.



This option is only active if the option **Recurse**  is set to a value other than 'Off'.



**Learn more about** 

*	:ref:`option-ODHCPLEX-recurse`  
*	:ref:`option-ODHCPLEX-recurse_iteration_limit`  
