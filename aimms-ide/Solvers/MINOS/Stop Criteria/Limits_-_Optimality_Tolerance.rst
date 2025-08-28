

.. _option-MINOS-optimality_tolerance:


Optimality Tolerance
====================



:Type:	Floating point number	
:Range:	[1e-15,1]	
:Default:	1e-6	



This option is used to judge the size of the reduced gradient be :math:`d_j = g_j - \pi^Ta_j`, where :math:`g_j` is the gradient of the objective function corresponding
to the :math:`j`-th variable, :math:`a_j` is the associated column of the constraint matrix (or Jacobian), and :math:`\pi` is the set of dual variables.

By construction, the reduced gradients for basic variables are always zero. Optimality will be declared if the reduced gradients for nonbasic variables
at their lower or upper bounds satisfy

.. math::

    \frac{d_j}{\| \pi \|} \geq - t \qquad \text{or} \qquad \frac{d_j}{\| \pi \|} \leq t,


respectively, and if :math:`\frac{d_j}{\| \pi \|} \leq t` for superbasic variables (where :math:`t` denotes the optimality tolerance).

In the above tests, :math:`\| \pi \|` is a measure of the size of the dual variables. It is included to make the tests independent of a scale factor on
the objective function. The quantity actually used is defined by

.. math::

    \| \pi \| = \max( \delta / \sqrt{m}, 1 ), \quad \text{where} \quad \delta = \sum \limits_i | \pi_i |,


so that only large scale factors are allowed for. If the objective is scaled down substantially, the test for optimality reduces to comparing :math:`d_j` against :math:`t`.



