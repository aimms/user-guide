

.. _option-AIMMS-rounding_compatibility:


Rounding Compatibility
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Not Selected	



This option specifies how AIMMS handles arithmetic functions such as :any:`round`, :any:`ceil`,
:any:`trunc` and :any:`floor`, with arguments with units. In AIMMS 3.0 until AIMMS 3.6 the value
of the argument of these functions were used with respect to their base unit. From AIMMS 3.7
onwards the value of the argument of these functions will be used with respect to the unit of
the argument. If this option has the value 'Not Selected' the AIMMS 3.0 method will be used
but a warning will be given upon first usage of these functions in a case where the argument
unit differs from the atomic unit.

Possible values are:

    *	Aimms 3 0 
    *	Aimms 3 7
    *	Not Selected


**Learn more about** 

*	:ref:`option-AIMMS-case_compression_level`  
*	:ref:`option-AIMMS-warning_rounding_ambiguity`  

