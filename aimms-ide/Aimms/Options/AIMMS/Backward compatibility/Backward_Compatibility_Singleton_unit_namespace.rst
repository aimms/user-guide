

.. _Options_Backward_Compatibility_Singleton_unit_namespace:


Singleton unit namespace
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



Up to AIMMS 3.8, unit symbols are stored in a single namespace separate from the identifier namespaces. With the introduction of AIMMS 3.9, unit symbols are still stored in separate namespaces but parallel to the identifier namespaces (for each library or module a separate namespace); Therefore, unit names now follow the same rules as identifier names.
The use of multiple namespaces for units makes it possible to have the same unit name, but with different interpretations, to be used in separate libraries or modules. In addition, two procedures can now declare both local unit parameters with the same name. On the other hand, applications developed in AIMMS 3.8 or previous versions, with quantity declarations inside libraries or modules may not compile anymore.


This option determines whether the old or new storing mechanism is used.



Changing this option requires that you save your project, close it and reopen it again; the data structures supporting unit analysis and conversion can then be rebuild.



Possible values are:



*	Off
*	On



