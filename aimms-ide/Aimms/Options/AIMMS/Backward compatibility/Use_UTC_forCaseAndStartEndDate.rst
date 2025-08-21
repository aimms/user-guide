

.. _option-AIMMS-use_utc_forcaseandstartenddate:


Use UTC forCaseAndStartEndDate
==============================

:Type:	Selection	
:Range:	The settings listed below	
:Default:	On in newly created projects, Off for existing projects	



When this option is active the default interpretation of time-strings is changed in two places:




#.  In cases: This allows loading the case in another time-zone than created without change of meaning
#.  In calendars: To prevent change of meaning when opening the model in another time-zone



Note that in all other cases (and when the option is off) the reference dates are local-noDST format. Since such usage is runtime, change of time-zone should not pose a problem if correctly used. e.g. One should be careful to feed CurrentToMoment a local time.



Possible values are:



*	Off
*	On



