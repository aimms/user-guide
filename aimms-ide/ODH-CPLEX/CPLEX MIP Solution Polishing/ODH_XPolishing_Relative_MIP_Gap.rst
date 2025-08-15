.. _ODH-CPLEX_XPolishing_Relative_MIP_Gap:


Polishing Relative MIP Gap
==========================



**Type**:	Floating point number	

**Range**:	[0,1]	

**Default**:	0	



This option sets a relative MIP gap after which CPLEX will stop branch-and-cut and begin polishing a feasible solution. The default value (0) is such that CPLEX does not invoke solution polishing by default. The relative MIP gap is calculated like this:



	``|bestnode-bestinteger| / (1e-10 + |bestinteger| ).`` 



CPLEX must have a feasible solution in order to start polishing. It must also have certain internal structures in place to support solution polishing. Consequently, when the criterion specified by this parameter is met, ILOG CPLEX begins solution polishing only after these starting conditions are also met. That is, there may be a delay between the moment when the criterion specified by this parameter is met and when solution polishing starts.



**Learn more about** 

*	:ref:`ODH-CPLEX_XPolishing_Absolute_MIP_Gap`  
