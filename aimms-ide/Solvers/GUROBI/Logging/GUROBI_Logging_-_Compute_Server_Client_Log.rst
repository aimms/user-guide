.. _option-GUROBI-compute_server_client_log:


Compute Server Client Log
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option turns logging on or off for Compute Server and the Web License Service (WLS). Possible values are:

    *	Off
    *	Error
    *	Information
    *	Verbose


**Remark** 

The logging can also be controlled using the procedure :any:`GMP::Solver::SetEnvironmentIntegerParameter` with
parameter value "CSClientLog".


**Learn more about** 

*   `Compute Server <https://how-to.aimms.com/Articles/277/277-aimms-with-gurobi.html#compute-server>`_
*	:any:`GMP::Solver::SetEnvironmentIntegerParameter`
