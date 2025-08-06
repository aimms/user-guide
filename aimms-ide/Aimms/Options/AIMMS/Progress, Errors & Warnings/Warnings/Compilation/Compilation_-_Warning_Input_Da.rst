

.. _Options_Compilation_-_Warning_Input_Da:


Warning Input Data Domain
=========================



Type:	Selection	

Range:	The settings listed below	

Default:	Common_warning_default	



This option determines what happens during compilation when initial data is referenced outside a conditional domain, depending on the following settings:




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




An example of such an input data domain violation arises in the following model fragment:



``SET:`` 

``identifier  : Cities`` 

``index    : c`` 

``definition  : data{Amsterdam,Paris} ;`` 

``PARAMETER:`` 

``identifier  : Population`` 

``index domain : c|ord(c)<2`` 

``initial data : data{Amsterdam: 0.7e6, Paris: 3e6} ;`` 



This option is only effective at the end of initialization; after running the procedure ``MainInitialization`` .



**Note** 

*	If you set this option to "Off" or "Warning", the data will be assigned to the elements that are outside the domain.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



