

.. _IPOPT_Restoration_phase_-_Required_infeasibility_reduction:


Required infeasibility reduction
================================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0.9	



This option determines the required reduction of infeasibility before leaving restoration phase. The restoration phase algorithm is performed, until a point is found that is acceptable to the filter and the infeasibility has been reduced by at least the fraction given by this option.

