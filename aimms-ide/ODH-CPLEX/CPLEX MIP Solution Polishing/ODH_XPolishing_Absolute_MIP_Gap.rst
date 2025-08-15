.. _ODH-CPLEX_XPolishing_Absolute_MIP_Gap:


Polishing Absolute MIP Gap
==========================



**Type**:	Floating point number	

**Range**:	[0,inf)	

**Default**:	0	



This option sets an absolute MIP gap (that is, the difference between the best integer objective and the objective of the best node remaining) after which CPLEX stops branch-and-cut and begins polishing a feasible solution. The default value (0.0) is such that CPLEX does not invoke solution polishing by default.



CPLEX must have a feasible solution in order to start polishing. It must also have certain internal structures in place to support solution polishing. Consequently, when the criterion specified by this parameter is met, CPLEX begins solution polishing only after these starting conditions are also met. That is, there may be a delay between the moment when the criterion specified by this parameter is met and when solution polishing starts.



**Learn more about** 

*	:ref:`ODH-CPLEX_XPolishing_Relative_MIP_Gap`  
