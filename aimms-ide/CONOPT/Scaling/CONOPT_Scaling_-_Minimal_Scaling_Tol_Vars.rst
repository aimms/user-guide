.. _CONOPT_Scaling_-_Minimal_Scaling_Tol_Vars:

Minimal Scaling Tolerance for Variables
=======================================



**Type**:	Floating point number	

**Range**:	[1e-8,1.0]	

**Default**:	1e-5	



This option specified the lower bound on x in x*Jac used during scaling. Rows are scaled so the largest term x*Jac is around 1. To avoid difficulties with models where Jac is very large and x very small, a lower bound of **Minimal Scaling Tolerance for Variables**  is applied to the x-term.



