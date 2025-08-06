

.. _Options_Math_program_inspector_-_unbound:


Unboundedness analysis bound
============================



Type:	Selection	

Range:	[1,1e20]	

Default:	1e7



When determining a substructure causing unboundedness, the Math Program Inspector temporary change all infinite bounds to this value. All variables and constraints whose value equals the 'unboundedness analysis bound' will be marked as contributing to the unboundedness. For badly scaled models, it might be necessary to increase the value of this option.



**Learn more about** 

*	:ref:`Diagnostic-Tools_AIMMS_Math_Program_Inspector`  






