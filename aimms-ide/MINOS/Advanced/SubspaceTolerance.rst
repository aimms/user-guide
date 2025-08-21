

.. _SubspaceTolerance:
.. _option-MINOS-subspace_tolerance:


Subspace Tolerance
==================



:Type:	Floating point number	
:Range:	[0.0001,1]	
:Default:	0.5	



The subspace tolerance t controls the extent to which optimization is confined to the current set of basic and superbasic variables (Phase 4 iterations), before one or more nonbasic variables are added to the superbasic set (Phase 3).



When a nonbasic variable xj is made superbasic, the resulting norm of the reduced-gradient vector (for all superbasics) is recorded. 
Let this be ``||`` ZTg0 ``||`` . (In fact, the norm will be :math:`|dj|`, the size of the reduced gradient for xj.)



Subsequent Phase 4 iterations continue at least until the norm of the reduced-gradient vector satisfies



	``||`` ZTg``||`` ≤  t``||`` ZTg0``||.`` 



(Here ``||`` ZTg``||`` is the size of the largest reduced-gradient among the superbasic variables.)



A smaller value of t is likely to increase the total number of iterations, but may reduce the number of basis changes. A larger value such as t = 0.9 may sometimes lead to improved overall efficiency, if the number of superbasic variables has to increase substantially between the starting point and an optimal solution.



Other convergence tests on the change in the function being minimized and the change in the variables may prolong Phase 4 iterations. This helps to make the overall performance insensitive to larger values of t. 

 

