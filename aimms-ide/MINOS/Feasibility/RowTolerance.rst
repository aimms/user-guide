

.. _option-MINOS-row_tolerance:


Row Tolerance
=============



:Type:	Floating point number	
:Range:	[1e-15,1]	
:Default:	1e-6	


This option specifies how accurately the nonlinear constraints should be satisfied. The default value is often appropriate,
since model data is often specified to about that accuracy.

Let :math:`R_{err}` be defined as the maximum component of the residual vector :math:`f(x) + Ay - b`, normalized by the size of the solution. Thus,

.. math::

    R_{err} = \frac{\| f(x) + Ay - b \|_{\infty}}{x_{norm}},



where :math:`x_{norm}` is a measure of the size of the basic and superbasic variables. The solution :math:`(x,y)` is regarded as
acceptably feasible if :math:`R_{err} \leq \epsilon`, where :math:`\epsilon` denotes the value of this option.



If the problem functions are known to be of low accuracy, a larger row tolerance may be appropriate.



