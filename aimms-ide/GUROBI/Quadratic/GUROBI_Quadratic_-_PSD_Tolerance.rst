.. _option-GUROBI-psd_tolerance:


PSD Tolerance
=============



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e-6	



This option specifies the positive semi-definite tolerance (QP/MIQP only). It sets a limit on the amount of diagonal perturbation that the optimizer is allowed to perform on the Q matrix in order to correct minor PSD violations. If a larger perturbation is required, the optimizer will terminate with an error.



