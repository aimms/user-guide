.. _option-GUROBI-concurrent_method:


Concurrent Method
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls the methods used by the concurrent continuous solver. Possible values are:



*	Automatic
*	Barrier, dual and primal simplex
*	Barrier and dual simplex
*	Barrier and primal simplex
*	Dual and primal simplex




This option is only used when solving a continuous model or the root node of a MIP model, while the option **Method**  is set to 'Opportunistic concurrent' or 'Deterministic concurrent', or when calculating sensitivity ranges and the option **Sensitivity Method**  is set to 'Opportunistic concurrent' or 'Deterministic concurrent'.





**Learn more about** 

*	:ref:`option-GUROBI-method` 
*	:ref:`option-GUROBI-sensitivity_method` 
