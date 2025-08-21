

.. _option-AIMMS-database_translate_case:


Database Translate Case
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Keep	



Some database management systems (for example Oracle) convert all table and column names to lower or upper case when an external database is imported, but still use case sensitive string comparison when AIMMS searches through the structure of a database in such a database management system. 



This option determines the way table and column names are converted during communication between AIMMS and the database management system. Possible values are:



*	Lower (convert all table and column names to lower case)
*	Keep (do not convert the table and column names)
*	Upper (convert all table and column names to upper case)



