

.. _Options_Database_String_Valued_Foreign_Keys:


Database String Valued Foreign Keys
===================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Ignore	



When this option is set to 'Check', AIMMS automatically determines, during database write actions, whether the written columns are referencing other tables as foreign keys.



This determination itself may be expensive in terms of performance (depending on database vendor). The option allows you to skip this test (runtime; until changed again). If a table has string valued columns which are foreign keys, NULL values should be written to the database for these columns in case of empty labels instead of the empty string ("").



Possible values are:



*	Ignore: All empty strings will be written as empty strings.
*	Check: AIMMS will request the foreign key information from the database. Only string valued foreign key columns will be written as NULL.
*	Assume: All empty strings will be written as NULL values.
