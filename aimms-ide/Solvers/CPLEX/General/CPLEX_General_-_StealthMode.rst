.. _option-CPLEX-stealth_mode:


Stealth Mode
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Normal	



By default, AIMMS installs CPLEX callback routines which are used to pass progress information, to run certain AIMMS callback
routines, and to give the user the possibility to interrupt the solve. If the value of this option equals 'Fast' then these
CPLEX callback routines are not installed. As a consequence the solve might become significantly faster. However the disadvantages are:

    *   The :ref:`aimmshelp12-progress_window` will not be updated during the solve;
    *   The solve cannot be interrupted;
    *   No callback will be made to AIMMS procedures that are installed with the Mathematical Program suffices ``CallbackProcedure``,``CallbackTime``  or ``CallbackStatusChange`` (or installed with the GMP routines :any:`GMP::Instance::SetCallbackIterations`, :any:`GMP::Instance::SetCallbackTime` or :any:`GMP::Instance::SetCallbackStatusChange`).


Possible values are:

    *	Normal
    *	Fast


**Note** 


*   If the value of this option is set to 'Fast' then still a callback will be made to AIMMS procedures installed with the GMP routines :any:`GMP::Instance::SetCallbackAddCut`, :any:`GMP::Instance::SetCallbackBranch`, :any:`GMP::Instance::SetCallbackHeuristic`, :any:`GMP::Instance::SetCallbackCandidate` or :any:`GMP::Instance::SetCallbackIncumbent`. (Same for a callback installed with the Mathematical Program suffix ``CallbackIncumbent``.)


**Learn more about** 

*	:ref:`option-AIMMS-progress_time_interval` 

