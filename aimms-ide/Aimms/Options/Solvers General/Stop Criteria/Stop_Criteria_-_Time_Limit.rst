

.. _option-AIMMS-time_limit:


Time Limit
==========



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	:ref:`Miscellaneous_Maxint` 	



After Time Limit CPU seconds have elapsed, solution procedures are interrupted and the current solution is returned to AIMMS.


**Note** 

*	This option can be modified from within a callback within :ref:`SolverGurobi` (version 12.0 or higher) using the procedure :any:`GMP::SolverSession::SetOptionValue`.
