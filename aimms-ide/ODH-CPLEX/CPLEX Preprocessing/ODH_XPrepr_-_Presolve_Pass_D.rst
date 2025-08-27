.. _option-ODHCPLEX-presolve_pass_dual:


Presolve Pass Dual
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines if CPLEX Presolve should pass the primal or dual LP problem to the LP optimization algorithm. By default, CPLEX chooses automatically. If this option is set to "Off", then the CPLEX presolve algorithm is applied to the primal problem, and the resulting primal problem is passed to the optimizer. If this option is set to "On", then the CPLEX presolve algorithm is applied to the primal problem, but the resulting dual problem is passed to the optimizer. This is a useful technique for problems with more constraints than variables. Possible values are:



    *	Off
    *	Automatic
    *	On



