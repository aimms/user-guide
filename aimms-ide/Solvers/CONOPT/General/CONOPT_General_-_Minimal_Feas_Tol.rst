.. _option-CONOPT-minimal_feasibility_tolerance:

Minimal Feasibility Tolerance
=============================



:Type:	Floating point number	
:Range:	[3e-13,1e-5]
:Default:	4e-10	



This option determines the mimumum feasibility tolerance (after scaling).



The feasibility tolerance used by CONOPT is dynamic. As long as we are far from the optimal solution and make large steps it is not necessary to compute intermediate solutions very accurately. When we approach the optimum and make smaller steps we need more accuracy. This option specifies the lower bound on the dynamic feasibility tolerance and the option **Minimal Feasibility Tolerance**  the upper bound.



**Learn more about** 

*	:ref:`option-CONOPT-maximal_feasibility_tolerance`  



