.. _ODH-CPLEX_XMIP_Solp_-_Pool_Abs_Obj_Gap:


Pool Absolute Objective Gap
===========================



**Type**:	Floating point number	

**Range**:	[0,1e75]	

**Default**:	1e75	



This option sets an absolute tolerance on the objective value for the solutions in the solution pool. Solutions that are worse (either greater in the case of a minimization, or less in the case of a maximization) than the objective of the incumbent solution according to this measure are not kept in the solution pool.



Values of the solution pool absolute gap and the solution pool relative gap may differ: For example, you may specify that solutions must be within 15 units by means of the solution pool absolute gap and also within 1% of the incumbent by means of the solution pool relative gap. A solution is accepted in the pool only if it is valid for both the relative and the absolute gaps.



The solution pool absolute gap option can also be used as a stopping criterion for the populate procedure: if populate cannot enumerate any more solutions that satisfy this objective quality, then it will stop. In the presence of both an absolute and a relative solution pool gap option, populate will stop when the smaller of the two is reached.



This option has only meaning if the option **Do** **Populate**  is switched on.



**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_Solp_-_Do_Populate`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Rel_Obj_Gap`  
