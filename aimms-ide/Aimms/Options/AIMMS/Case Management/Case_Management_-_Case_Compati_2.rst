

.. _option-AIMMS-case_compatibility:


Case Compatibility
==================



:Type:	Selection	
:Default:	'Aimms 4 80' in newly created projects; 'Aimms 3 14' for converted old AIMMS projects	



This option determines whether the cases should be compatible with older versions of AIMMS.
Possible values are:

    *	Aimms 3 14
    *	Aimms 4 80

To be able to make constant improvements to AIMMS, it is sometimes necessary to change the
way cases are stored. It is always possible to read cases made with an older AIMMS version,
but it is by default not always possible to read cases made with a newer AIMMS version. If
you want to be able to read cases in an older AIMMS version, you should modify this option. 

For new projects the prefered setting is 'Aimms 4 80' because it improves ordering of
identifiers in a case, for better performance. Also, this setting is required if you want to
use the Native_Linux or Native_Windows character encodings, as controlled by the option
**Case String Character Set**.

For AIMMS projects orginally created in AIMMS 4.79 or older, that are converted to a newer
AIMMS version, this option will be set to 'Aimms 3 14'.


**Remark** 

We advice you to set this option to older versions only if the cases need to be compatible with
older versions of AIMMS.


**Learn more about** 

*	:ref:`option-AIMMS-case_compression_level`  
*	:ref:`option-AIMMS-case_string_character_set`

