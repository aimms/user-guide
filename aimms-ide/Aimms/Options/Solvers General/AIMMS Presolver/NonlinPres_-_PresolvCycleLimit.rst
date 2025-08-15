

.. _Options_NonlinPres_-_PresolvCycleLimit:


Presolve Cycle Limit
====================



:Type:	Integer	
:Range:	{0..:ref:`Miscellaneous_Maxint` }	
:Default:	10	



During the first cycle the AIMMS Presolver processes all linear and/or nonlinear constraints to improve the bounds of the variables (using Feasibility-Based Bound Tightening). If one of the variable bounds is changed then all constraints containing that variable are marked and will be processed in the next cycle. Surely, an improved bound of a variable might imply better bounds on some other variables that belong to the same constraint. This could lead to an infinite sequence of cycles. This option limits the amount of cycles of processing constraints after one of the variable bounds changed.



The AIMMS Presolver might do one additional iteration of improving the variable bounds if the option **Presolve Dual Reductions**  is enabled. This additional iteration does not count towards the cycle limit.



**Learn more about** 

*	:ref:`Options_NonlinPres_-_Presolve_Dual_Reductions` 
