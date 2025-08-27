

.. _option-AIMMS-duplicate_row_update_protection:


Duplicate Row Update Protection
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



When this option is set to 'On', an error will be issued when the user writes to a database table and the write action results in duplicate rows to be updated in the database. This situation is caused by using a primary key in the mapping of a database table, that is not exactly the same as the physical primary key in the database table itself. After this error, AIMMS automatically rolls back the changes which resulted from the write statement.



Possible values are:



    *	On
    *	Off






