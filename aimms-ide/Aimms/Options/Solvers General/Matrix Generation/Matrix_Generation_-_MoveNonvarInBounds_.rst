

.. _option-AIMMS-move_nonvar_level_within_bounds:


Move Nonvar Level Within Bounds
===============================


:Type:	Selection	
:Range:	The settings listed below
:Default:	Off	

With this option you specify what to do with a variable for which:

    1. the nonvar status is not 0, and
    2. the current level value is not within the bounds of the variable.


Possible values are:

    *	Off
    *	On

If the option is switched off, then the level value remains unchanged and thus the generated mathematical program will work with this 'out of bounds' value,
If the option is switched on, then prior to generation, the level value is changed to the value of the nearest bound.


**Note** 

*	This option is only used by the new generator, as controlled by the option **Disable New Mathprog Generator**.
*	This option was added in AIMMS version 25.7.1.


**Learn more about** 

*	:ref:`option-AIMMS-disable_new_mathprog_generator`
