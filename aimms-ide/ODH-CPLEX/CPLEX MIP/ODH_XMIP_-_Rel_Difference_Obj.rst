.. _ODH-CPLEX_XMIP_-_Rel_Difference_Obj:


Relative Difference Objective
=============================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0	



The value of this option is used to update the cutoff each time a mixed integer solution is found. The value is multiplied by the absolute value of the integer objective and subtracted from (added to) the newly found integer objective when minimizing (maximizing). This forces the mixed integer optimization to ignore integer solutions that are not at least this amount better than the one found so far. The **Relative Objective Difference** option can be adjusted to improve problem solving efficiency by limiting the number of nodes; however, setting this option at a value other than zero (the default) can cause some integer solutions, including the true integer optimum, to be missed. If both this option and the option **Difference Objective**  are nonzero, the value of the option **Difference Objective**  will be used.



**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_Difference_Object`  



