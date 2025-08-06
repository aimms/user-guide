

.. _Options_Enccoding_Options_-_external_dll_AIMMS_reference:


External dll AIMMS reference
============================



Type:	Selection	

Range:	{ ASCII, Unicode, none }	

Default:	None	



External dll's, that use the AIMMS API, are linked against 

*	libAimms.dll when using ASCII or Unicode AIMMS 3.13 or older
*	libAimms3.dll when using AIMMS 3.14 or newer.

The AIMMS API's of AIMMS 3.13 and AIMMS 3.14 differ because from AIMMS 3.14 onwards, there are no longer separate AIMMS releases for ASCII and Unicode environments. Existing external DLL's, that are linked against either AIMMS 3.13 ASCII or AIMMS 3.13 Unicode, or an older functional release, need not be recompiled and linked; this option allows the old AIMMS API to be reused by your existing DLL's in your AIMMS 3.14 project. 





Possible values of this option are:

*	ASCII, use this if your DLL's are linked against ASCII AIMMS 3.13 or older.
*	Unicode, use this if your DLL's are linked against Unicode AIMMS 3.13 or older.
*	None, use this if you do not have any DLL's or if you can compile and link them.




This option is typically set during the conversion of an existing AIMMS 3.13 project to AIMMS 3.14 by AIMMS 3.14 itself.




