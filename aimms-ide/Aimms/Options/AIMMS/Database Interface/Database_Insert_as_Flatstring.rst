

.. _Options_Database_Insert_as_Flatstring:


Database Insert as Flatstring
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Default	



When writing data to a database via the ODBC Driver, parameters can be used for each row, but for some vendors and ODBC drivers this can be slow. Therefor AIMMS offers an altenative flat-string technique for a few vendors. This alternative is currently available for MySQL, MS SQLServer and PostgreSQL. Based on performance experiments, the default for MySQL and Postgres is to using this flatstring technique, but for all three of these you can adjust this default by setting the option to On or Off explicitly.



Possible values are:



*	On
*	Default (which translates to: for MySql: On, for PostgreSQL: On, MS SQLServer: Off)
*	Off
