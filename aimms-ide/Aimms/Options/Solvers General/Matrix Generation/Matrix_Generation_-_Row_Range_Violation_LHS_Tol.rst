

.. _option-AIMMS-row_range_violation_left_hand_side_tolerance:


Row Range Violation Left Hand Side Tolerance
============================================



:Type:	Floating point number	
:Range:	[0.0, 1.0]	
:Default:	0.001


If the option **Row Range Violation Left Hand Side** is switched on then, during the generation
of a mathematical program, individual constraints are checked for feasibility by computing the
range of the left-hand-side and comparing it to the right-hand-side. This option specifies the
tolerance used for this check. If the difference between the left-hand-side and the right-hand-side
is larger than the value of this option then the constraint is marked as infeasible.


**Learn more about** 

*	:ref:`option-AIMMS-row_range_violation_left_hand_side` 
