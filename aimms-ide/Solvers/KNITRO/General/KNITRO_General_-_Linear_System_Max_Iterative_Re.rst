.. _option-KNITRO-linear_system_max_iterative_refinements:


Linear System Max Iterative Refinements
=======================================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	2	



Indicates the maximum allowable number of iterative refinement steps applied when a linear system is solved inside Knitro. Iterative refinement steps may be applied when there are significant errors (e.g. large residuals) in the linear system solves. Applying more iterative refinement steps may improve the numerical accuracy of the linear solves at extra cost.

