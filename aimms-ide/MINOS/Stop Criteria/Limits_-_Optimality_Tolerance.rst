

.. _option-MINOS-optimality_tolerance:


Optimality Tolerance
====================



:Type:	Floating point number	
:Range:	[1e-15,1]	
:Default:	1e-6	



This option is used to judge the size of the reduced gradient be dj = gj - pTaj, where gj is the gradient of the objective function corresponding to the j-th variable, aj is the associated column of the constraint matrix (or Jacobian), and p is the set of dual variables.



By construction, the reduced gradients for basic variables are always zero. Optimality will be declared if the reduced gradients for nonbasic variables at their lower or upper bounds satisfy



dj ``/ ||`` p``|| >= - t`` or  dj ``/ ||`` p``|| <= t`` ``,`` 



respectively, and if dj``/ ||`` p``|| <= t`` for superbasic variables (where t denotes the optimality tolerance).



In the above tests, ``||`` p``||``  is a measure of the size of the dual variables. It is included to make the tests independent of a scale factor on the objective function. The quantity actually used is defined by



``||`` p ``|| =`` max{ d / Öm, 1 },  where :math:`d = åi  | pi |`,



so that only large scale factors are allowed for. If the objective is scaled down substantially, the test for optimality reduces to comparing dj against t.



