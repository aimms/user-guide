

.. _Options_DatabaseInterface-WarningD:


Warning Database Non Official Key in Mapping
============================================



Type:	Selection	

Range:	The settings listed below	

Default:	Common_warning_default	



When this option is not set to 'off', a warning (or error) will be issued when the user tries to read from or write to a database table, using a primary key in the mapping that is not exactly the same as the official primary key in the database table itself. Possible values are:




.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector.
   * - *	Common_warning_default
     - Take action depending on the option 'Common warning default'.
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler.
   * - *	Strict_warning_default
     - Take action depending on the option 'Strict warning default'.
   * - *	Error
     - Issue an error.
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off






