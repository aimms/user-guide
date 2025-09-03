

.. _option-AIMMS-warning_side_effects:


Warning Side Effects
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Error	



This option determines what happens during compilation when a procedure, referenced inside the definition of a set or a parameter, has a side effect; this situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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




An example of such a side effect occurs in the following model, where the parameter "TotalCosts" is defined via the internal procedure "ComputeCosts". A side effect of this procedure is the change of the global parameter "SomeParameter".



``PARAMETER:`` 

``identifier : TotalCosts`` 

``definition : ComputeCosts(TotalCosts,5) ;`` 

``PARAMETER:`` 

``identifier : SomeParameter ;`` 

``PROCEDURE`` 

``identifier : ComputeCosts`` 

``arguments : Costs,Production`` 

``PARAMETER:`` 

``identifier : Costs`` 

``property  : Output ;`` 

``PARAMETER:`` 

``identifier : Production`` 

``property  : Input ;`` 

``body :`` 

``Costs:=2*Production+10;`` 

``SomeParameter:=1;`` 

``ENDPROCEDURE ;`` 



**Note** 

*	If you set this option to "Off" or "Warning", then it is not predictable how these side effects will influence the execution of the model.
*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 






