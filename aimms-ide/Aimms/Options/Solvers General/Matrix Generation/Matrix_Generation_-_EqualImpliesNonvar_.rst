

.. _option-AIMMS-equal_bounds_imply_nonvar:


Equal Bounds Imply Nonvar
=========================



:Type:	Selection	
:Range:	The settings listed below
:Default:	Off	


With this option you can specify how variables for which the lower bounds equals the upper bound end up in a generated mathematical program.
Possible values are:

    *	Off
    *	On

If the option is switched off, then such a variable will appear as a 'frozen' column in the generated mathematical program.
If the option is switched on, then such a variable will not appear as a column in the generated mathematical program (similar as if the nonvar status is > 0).

**Remark**

If for a variable the lower bound equals the upper bound, **and** the nonvar status is not equal to 0, then the nonvar status is leading,
and thus this option will be ignored. For example if this option is switched on, the bounds are equal, but the nonvar is -1, then the
variable will appear as a frozen column in the generated mathematical program.


**Note** 

*	This option is only used by the new generator, as controlled by the option **Disable New Mathprog Generator**.
*	This option was added in AIMMS version 25.7.1.


**Learn more about** 

*	:ref:`option-AIMMS-disable_new_mathprog_generator`
