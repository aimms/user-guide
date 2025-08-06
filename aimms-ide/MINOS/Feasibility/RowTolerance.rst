

.. _RowTolerance:
.. _MINOS_RowTolerance:


Row Tolerance
=============



**Type** :	Floating point number	

**Range** :	[1e-15,1]	

**Default** :	1e-6	



This option specifies how accurately the nonlinear constraints should be satisfied. The default value is often appropriate, since model data is often specified to about that accuracy.



Let Rerr be defined as the maximum component of the residual vecor f(x) + Ay - b, normalizes by the size of the solution. Thus,



	Rerr = ``||``  f(x) + Ay - b ``||`` ¥ / xnorm,



where xnorm is a measure of the size of the basic and superbasic variables. The solution (x,y) is regarded as acceptably feasible if Rerr ≤ e, where e denotes the value of this option.



If the problem functions are known to be of low accuracy, a larger row tolerance may be appropriate.



