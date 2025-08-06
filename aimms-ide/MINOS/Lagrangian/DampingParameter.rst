

.. _DampingParameter:
.. _MINOS_DampingParameter:


Damping Parameter
=================



**Type** :	Floating point number	

**Range** :	[0.0001,1000]	

**Default** :	2.0



This option may assist convergence on problems that have highly nonlinear constraints. It is intended to prevent large relative changes between subproblem solutions (xk, lk) and (xk+1, lk+1). For example, the default value 2.0 prevents the relative change in either xk or lk from exceeding 200 per cent. It will not be active on well behaved problems.



This option is used to interpolate between the solutions at the beginning and end of each major iteration. Thus, xk+1 and lk+1 are changed to



	xk + s(xk+1 - xk)  	and  	lk + s(lk+1 - lk)



for some steplength s < 1. In the case of nonlinear equations (where the number of constraints is the same as the number of variables) this gives a damped Newton method.



