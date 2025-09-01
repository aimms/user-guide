

.. _option-AIMMS-small_data_updates_strategy:


Small Data Updates Strategy
===========================

:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	



This option can be used to activate a strategy in which small data updates are used to actually change the values of the
left-hand-side of an assignment. Possible values are:

    *	On
    *	Off


For some statements the default setting results in a significant performance improvement. If you feel that your assignment is
performing not as well as expected, you may attempt to switch the strategy by setting this option to 'Off'.

