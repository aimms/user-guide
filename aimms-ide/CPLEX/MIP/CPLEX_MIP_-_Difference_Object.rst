.. _CPLEX_MIP_-_Difference_Object:


Difference Objective
====================



**Type** :	Floating point number	

**Range** :	(-inf, inf)	

**Default** :	0	



The value of this option is used to update the cutoff each time a mixed integer solution is found. This absolute value will be subtracted from (added to) the newly found integer objective value when minimizing (maximizing). This forces the mixed integer optimization to ignore integer solutions that are not at least this amount better than the one found so far. The **Difference Objective**  option can be adjusted to improve problem solving efficiency by limiting the number of nodes; however, setting this option at a value other than zero (the default) can cause some integer solutions, including the true integer optimum, to be missed. Negative values for this option will result in some integer solutions that are worse than or the same as those previously generated, but will not necessarily result in the generation of all possible integer solutions.



