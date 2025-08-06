

.. _Options_Interface_-_Solution_Tolerance:


Solution Tolerance
==================



Type:	Floating point number	

Range:	[0,0.5]	

Default:	1e-007	



The solution values (in absolute sense) returned by the solver that are smaller than the value of this option, are translated to 0. However, AIMMS will not round the level value to 0 if that would result in a violation of a bound. For example, if the solver returns a level value of 1e-8 for some variable for which the lower bound is set to 1e-10 then AIMMS will not set the level value to 0 (and also not to 1e-10).



