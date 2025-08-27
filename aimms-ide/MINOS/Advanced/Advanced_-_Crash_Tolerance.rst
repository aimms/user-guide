

.. _option-MINOS-crash_tolerance:


Crash Tolerance
===============



:Type:	Floating point number	
:Range:	[0, 0.9999]	
:Default:	0.1	



The Crash tolerance r allows the starting procedure Crash to ignore certain "small" nonzeros in the constraint matrix whilesearching for a
triangular basis. For each column of :math:`A`, if :math:`\alpha_{max}` denotes the largest element in column :math:`j`, other nonzeros
:math:`\alpha_{ij}` in that column are ignored if :math:`| \alpha_{ij} | \leq \alpha_{max} \times r`.

When the value of this option is unequal to 0, the basis obtained by Crash may not be strictly triangular, but it is likely to be
nonsingular and almost triangular. The intention is to obtain a starting basis containing more columns of :math:`A` and fewer (arbitrary) slacks.
A feasible solution may be reached sooner on some problems.



**Learn more about** 

*	:ref:`option-MINOS-calling_crash_procedure`  



