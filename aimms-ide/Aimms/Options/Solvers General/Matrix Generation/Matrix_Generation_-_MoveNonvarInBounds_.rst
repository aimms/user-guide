

.. _option-AIMMS-move_nonvar_level_within_bounds:


Move Nonvar Level Within Bounds
===============================


:Type:	Selection	
:Range:	{ On, Off }
:Default:	Off	

With this option you specify what to do with a variable for which:
(1) the nonvar status is not 0, and
(2) the current level value is not within the bounds of the variable


If the option is switched off, then the level value remains unchanged and thus the generated mathematical program will work with this 'out of bounds' value,
If the option is switched on, then prior to generation, the level value is changed to the value of the nearest bound.



