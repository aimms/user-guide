

.. _option-IPOPT-factor_for_initial_bounds_relaxation:


Factor for initial bounds relaxation
====================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	1e-008	



This option specifies the factor for initial relaxation of the bounds. Before the start of the optimization, the bounds given by the user are relaxed. This option sets the factor for this relaxation. If it is set to 0 then bounds relaxation is disabled.

