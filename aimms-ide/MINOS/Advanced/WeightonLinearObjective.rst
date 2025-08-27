

.. _option-MINOS-weight_on_linear_objective:


Weight on Linear Objective
==========================



:Type:	Floating point number	
:Range:	[0,1e20]
:Default:	0	



This option invokes the so-called composite objective technique, if the first solution obtained is infeasible, and if the objective
function contains linear terms. While trying to reduce the sum of infeasibilities, the method also attempts to optimize the linear objective.


At each infeasible iteration, the objective function is defined to be 


.. math::

    \text{minimize} \sigma w(c^Tx) + \text{(sum of infeasibilities)},



where :math:`\sigma = 1` for minimization, :math:`\sigma = -1` for maximization, and :math:`c` is the linear objective.


If an "optimal" solution is reached while still infeasible, :math:`w` is reduced by a factor of 10. This helps to allow for the possibility
that the initial :math:`w` is too large. It also provides dynamic allowance for the fact that the sum of infeasibilities is tending towards zero.


The effect of :math:`w` is disabled after 5 such reductions, or if a feasible solution is obtained. 



