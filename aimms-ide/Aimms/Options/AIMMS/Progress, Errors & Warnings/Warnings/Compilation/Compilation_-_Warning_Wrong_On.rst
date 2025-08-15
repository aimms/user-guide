

.. _Options_Compilation_-_Warning_Wrong_On:


Warning Wrong Onlyif Symbol
===========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Strict_warning_default	



``Although the symbol "|" in AIMMS 2.20 could be used for both the "only if" operator and the "such that" operator in index domains, in AIMMS 3.0, the symbol "|" just stands for the "such that" operator, and should not be used for the "only if" operator, for which the symbol reads "$". This option determines what happens during the compilation of expressions that still use the "|" symbol for the ONLYIF operator instead of "$". This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:`` 




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




**Note** 

*	If this option has the value "Off" or "Warning", then "|" as symbol for "only if" is translated to "$".
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



