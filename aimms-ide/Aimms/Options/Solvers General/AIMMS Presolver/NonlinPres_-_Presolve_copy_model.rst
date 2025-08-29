

.. _option-AIMMS-presolve_copy_model:


Presolve Copy Model
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether the AIMMS Presolver should make a copy of the generated math program and apply presolve changes to this copy. Possible values are:

    *	Off
    *	On


If this option is switched off then the AIMMS Presolver will apply presolve changes directly to the
original generated math program, and undo these changes after the solve. For large models, AIMMS will
consume less memory if this option is switched off. Switching off this option will also make the AIMMS
Presolver faster.

Currently, this option is only effective for linear models for which the option **Linear Presolve** has
been enabled. The AIMMS Presolver will always make a copy of the generated math program if the model is nonlinear.


**Note** 

*	The AIMMS Presolver will always apply presolve changes directly to the original generated math program for linear models with a cut, lazy constraint or branch callback installed, even if this option is switched on.
*	In AIMMS version 4.82 and older, the AIMMS Presolver always made a copy of the generated math program.


**Learn more about** 

*	:ref:`option-AIMMS-linear_presolve` 
