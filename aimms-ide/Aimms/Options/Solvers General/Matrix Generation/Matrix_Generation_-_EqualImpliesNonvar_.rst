

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
If the option is switched on, then such a variable will not appear as a column in the generated mathematical program (similar as if the nonvar status is > 0),
unless the option **Eliminate Nonvar Columns** is switched off.

The default is off, because to support this behavior extra steps are needed that effect the total generation time and for LP or MIP models it is not that important for the generated mathematical program. However, for NLP models in particular, we recommend enabling it. It can reduce both model size and the number of nonlinearities, which helps solver performance.

**Remark**

If for a variable the lower bound equals the upper bound, **and** the nonvar status is not equal to 0, then the nonvar status is leading,
and thus this option will be ignored. For example if this option is switched on, the bounds are equal, but the nonvar is -1, then the
variable will appear as a frozen column in the generated mathematical program.


**Note** 

*	This option is only used by the new generator, as controlled by the option **Disable New Mathprog Generator**.
*	This option was added in AIMMS version 25.7.1.
*	If this option is enabled, then the option **Move Nonvar Level Within Bounds** is automaticlly also treated as being enabled.


**Learn more about** 

*	:ref:`option-AIMMS-disable_new_mathprog_generator`
*	:ref:`option-AIMMS-eliminate_nonvar_columns`
*	:ref:`option-AIMMS-move_nonvar_level_within_bounds`

