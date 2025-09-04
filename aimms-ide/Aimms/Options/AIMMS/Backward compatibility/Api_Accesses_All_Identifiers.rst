

.. _option-AIMMS-api_accesses_all_identifiers:


Api Accesses All Identifiers
============================



:Type:	Selection	
:Range:	The settings listed below
:Default:	Off	



This option determines whether handles to identifiers declared inside a library, but not present in the
interface of that library, are allowed to be created via the function AimmsIdentifierHandleCreate. The
default behaviour is to insist that handles are only created for identifiers inside the interface.

Possible values are:

    *	On (AIMMS ignores the interface when creating handles)
    *	Off (AIMMS adheres to the interface of a library when creating identifiers)


**Remark** 

This option becomes obsolete when a revised mechanism is available in the language for protecting private identifiers of a library.

