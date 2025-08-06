

.. _Options_Api_Accesses_All_Identifiers:


Api Accesses All Identifiers
============================



Type:	Selection	

Range:	{ on, off }	

Default:	off	



This option determines whether handles to identifiers declared inside a library, but not present in the interface of that library, are allowed to be created via the function AimmsIdentifierHandleCreate. From AIMMS 3.13 and upwards, the default behaviour is to insist that handles are only created for identifiers inside the interface.



*	off (default)	AIMMS adheres to the interface of a library when creating identifiers.
*	on			AIMMS ignores the interface when creating handles.







**Remark** 


This option will become obsolete when a revised mechanism is available in the language for protecting private identifiers of a library.







