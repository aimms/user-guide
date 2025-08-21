.. _option-GUROBI-barrier_qcp_convergence_tolerance:


Barrier QCP Convergence Tolerance
=================================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-6	



This option controls barrier termination when solving a QCP model. The barrier solver terminates when the relative difference between the primal and dual objective values is less than the specified tolerance. Tightening this tolerance may lead to a more accurate solution, but it may also lead to a failure to converge.

