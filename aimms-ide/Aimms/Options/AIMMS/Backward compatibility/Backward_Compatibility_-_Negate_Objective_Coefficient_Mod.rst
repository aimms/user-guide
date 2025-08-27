

.. _option-AIMMS-negate_objective_coefficient_modifications:


Negate Objective Coefficient Modifications
==========================================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	Off	



If this option is switched on then coefficient values passed to the procedures GMP::Coefficient::Set and GMP::Coefficient::SetMulti will automatically be multiplied by -1 if the row (passed as argument to these procedures) contains the objective variable. Possible values are:



    *	Off
    *	On




**Note** 

*	In AIMMS 3.13 and older versions, coefficients were multiplied by -1 if the row contained the objective variable. Since AIMMS 3.14 this is no longer the case (by default).
