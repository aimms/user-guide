

.. _option-AIMMS-solver_listing_messages:


Solver Listing Messages
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines if and which messages of the solver are included in the solver listing file. Possible values are:



    *	Never
    *	Error
    *	Warning
    *	Remark
    *	All
    *	Automatic


If this option equals 'Automatic' then AIMMS will use the value 'Remark' if the project runs in developer mode,
and the value 'Never' if the project runs in end-user mode (which is the case if the project runs on the AIMMS
Cloud or AIMMS PRO On-Premise).


**Note**

*	The default of this option was changed from 'Never' to 'Automatic' in AIMMS 26.4.


**Learn more about**

*	:ref:`option-AIMMS-solver_listing`
*	:ref:`option-AIMMS-solver_window_messages`


