

.. _Advanced_-_Crash_Tolerance:
.. _MINOS_Advanced_-_Crash_Tolerance:


Crash Tolerance
===============



**Type**:	Floating point number	

**Range**:	[0, 0.9999]	

**Default**:	0.1	



The Crash tolerance r allows the starting procedure Crash to ignore certain "small" nonzeros in the constraint matrix while searching for a triangular basis. For each column of A, if amax denotes the largest element in column j, other nonzeros aij in that column are ignored if | aij | <= amax x r.



When the value of this option is unequal to 0, the basis obtained by Crash may not be strictly triangular, but it is likely to be nonsingular and almost triangular. The intention is to obtain a starting basis containing more columns of A and fewer (arbitrary) slacks. A feasible solution may be reached sooner on some problems.



**Learn more about** 

*	:ref:`MINOS_Advanced_-_Calling_Crash`  



