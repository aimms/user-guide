.. _option-KNITRO-status_file_display:


Status File Display
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Every 10 major iterations	



If this option is switched on, a file with the name 'knitro.log' is created (in the log-directory). In this file an iteration log and error messages are printed. Possible values are:



    *	None
    *	Summary
    *	Every 10 major iterations
    *	Each major iteration
    *	Each major and minor iteration
    *	All plus variable values
    *	All plus complete solution


**Note**

*	The default of this option was changed from 'None' to 'Every 10 major iterations' in AIMMS 26.4.

