.. _option-GUROBI-work_limit:


Work Limit
==========



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100



This option limits the total work expended (in work units). Optimization returns with a ResourceInterrupt solver status if the limit is exceeded.



In contrast to a time limit, work limits are deterministic. This means that on the same hardware and with the same option settings, a work limit will stop the optimization of a given model at the exact same point every time. One work unit corresponds very roughly to one second on a single thread, but this greatly depends on the hardware on which Gurobi is running and the model that is being solved.



Note that the optimization may not stop immediately upon hitting the work limit. It will stop when the optimization is next in a deterministic state.



