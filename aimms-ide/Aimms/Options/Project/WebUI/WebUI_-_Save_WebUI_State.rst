

.. _Options_WebUI_-_Save_WebUI_State:


Save WebUI State
================



Type:	Selection	

Range:	The settings listed below	

Default:	Never



This option controls whether the WebUI state is saved when the application is run under AIMMS PRO. Possible values are:



*	Never
*	Upon session termination




If this option is set to 'Upon session termination', then the WebUI state will be saved in the PRO Storage area upon closing the application (and the session termination by the PRO server). In this case, the saved state will be restored upon re-starting the application from the AIMMS PRO portal.





If this option is set to 'Never', then the WebUI state is not saved upon session termination.

