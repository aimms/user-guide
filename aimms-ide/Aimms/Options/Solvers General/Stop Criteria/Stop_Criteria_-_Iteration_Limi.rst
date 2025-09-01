

.. _option-AIMMS-iteration_limit:


Iteration Limit
===============



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	:ref:`Miscellaneous_Maxint` 	



After Iteration Limit iterations, the iterative solution procedures are interrupted and the current solution is returned to AIMMS.


**Note** 

*	In case the solver makes a distinction between minor and major iterations, this option gives the total number of minor iterations allowed.
*	For :ref:`SolverCPLEX` and :ref:`SolverGurobi`, if this option is set to its default value (or any value greater than 2,100,000,000) then the actual iteration limit used by both solvers will be a value that is larger than 9e18.
*	For :ref:`SolverCOPT` the iteration limit is only used by the barrier algorithm.

