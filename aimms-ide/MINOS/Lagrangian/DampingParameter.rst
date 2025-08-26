

.. _option-MINOS-damping_parameter:


Damping Parameter
=================



:Type:	Floating point number	
:Range:	[0.0001,1000]	
:Default:	2.0



This option may assist convergence on problems that have highly nonlinear constraints. It is intended to prevent large relative
changes between subproblem solutions :math:`(x_k, \lambda_k)` and :math:`(x_{k+1}, \lambda_{k+1})`. For example, the default value 2.0 prevents the
relative change in either :math:`x_k` or :math:`\lambda_k` from exceeding 200 per cent. It will not be active on well behaved problems.

This option is used to interpolate between the solutions at the beginning and end of each major iteration. Thus, :math:`(x_{k+1}`
and :math:`(\lambda_{k+1}` are changed to

.. math::

    x_k + \sigma(x_{k+1} - x_k) \qquad \text{and} \qquad \lambda_k + \sigma(\lambda_{k+1} - \lambda_k)


for some steplength :math:`\sigma < 1`. In the case of nonlinear equations (where the number of constraints is the same as the
number of variables) this gives a damped Newton method.



