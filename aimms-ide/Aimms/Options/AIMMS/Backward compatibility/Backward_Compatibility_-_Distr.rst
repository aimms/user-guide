

.. _option-AIMMS-distribution_compatibility:


Distribution Compatibility
==========================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	AIMMS 3 4	



For various distribution functions the number of arguments and interpretation of arguments has changed in AIMMS 3.4. This option specifies which interpretation should be used. When the value of the option is 'AIMMS 3 0' the old method will be used, when the value is 'AIMMS 3.4' the new method will be used. When the option is set to 'Not Selected' the new method will be used and a warning message will be displayed. Possible values are:



*	AIMMS 3 0
*	AIMMS 3 4
*	Not Selected




**Remark** 


When a model made in an old AIMMS version (older than AIMMS 3.4) is opened in AIMMS 3.4 or later the value of this option will be set to 'Not Selected', forcing the user to make a choice between the 'AIMMS 3 0' and 'AIMMS 3 4' method. When a new model is made in AIMMS 3.4 or later the value of this option will be set to AIMMS 3 4.







