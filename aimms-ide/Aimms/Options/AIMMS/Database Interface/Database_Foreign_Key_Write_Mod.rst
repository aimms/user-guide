

.. _option-AIMMS-database_foreign_key_handling:


Database Foreign Key Handling
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Check	



When this option is set to 'Check', AIMMS automatically determines, during database write actions, whether the written columns are referred to as foreign keys.

This determination itself may be expensive in terms of performance (at least for Oracle databases). The option allows you to skip this test (runtime; until changed again). If the value is 'Assume', AIMMS will use a less efficient foreign-key-safe algorithm. When the value is 'Ignore', AIMMS will use a faster algorithm. This, however, may cause errors and/or data loss when used while foreign keys are active.    



Possible values are:



    *	Ignore
    *	Check
    *	Assume
