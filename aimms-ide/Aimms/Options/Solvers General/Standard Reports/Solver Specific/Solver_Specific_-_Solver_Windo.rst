

.. _option-AIMMS-solver_window_messages:


Solver Window Messages
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines if and which messages of the solver are included in the :ref:`aimmshelp13-Messages_Window`. Possible values are:

    *	Never
    *	Error
    *	Warning
    *	Remark
    *	All
    *	Automatic


If this option equals *Automatic* then AIMMS will use the value *Error* if the project runs in developer mode,
and the value *Remark* if the project runs in end-user mode (which is the case if the project runs on the AIMMS
Cloud or AIMMS PRO On-Premise).


**Note**

*	On the AIMMS Cloud or AIMMS PRO On-Premise the solver logging is printed in the session log.
*	The default of this option was changed from 'Error' to 'Automatic' in AIMMS 26.4.


**Learn more about**

*	:ref:`option-AIMMS-solver_listing_messages`
