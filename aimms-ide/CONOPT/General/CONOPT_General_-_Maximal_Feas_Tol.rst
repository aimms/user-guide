.. _CONOPT_General_-_Maximal_Feas_Tol:

Maximal Feasibility Tolerance
=============================



**Type** :	Floating point number	

**Range** :	[1e-10,0.001]	

**Default** :	1e-7	



This option determines the maximum feasibility tolerance (after scaling).



The feasibility tolerance used by CONOPT is dynamic. As long as we are far from the optimal solution and make large steps it is not necessary to compute intermediate solutions very accurately. When we approach the optimum and make smaller steps we need more accuracy. This option specifies the upper bound on the dynamic feasibility tolerance and the option **Minimal Feasibility Tolerance**  the lower bound.



**Learn more about** 

*	:ref:`CONOPT_General_-_Minimal_Feas_Tol`  



