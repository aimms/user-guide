

.. _option-AIMMS-solver_workspace:


Solver Workspace
================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	0	



This option determines how much memory the solver may allocate as workspace. It is measured in Mbytes. If Solver Workspace
is zero, then the solver decides itself how much workspace it needs.

The value 'inf' has a special meaning. On a 64-bits machine it is translated into 218.

This option is not supported by :ref:`SolverCPLEX`; for this solver its option **Working Memory Limit** is used instead.


**Learn more about** 


* :ref:`option-CPLEX-working_memory_limit`


