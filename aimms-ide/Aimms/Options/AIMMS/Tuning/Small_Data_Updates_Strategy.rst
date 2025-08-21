

.. _option-AIMMS-small_data_updates_strategy:


Small Data Updates Strategy
===========================

:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	



In AIMMS 4.2, the strategy to actually change the values of the left-hand-side of an assignment can be modified by this option.

For some statements this new strategy results in a significant performance improvement. If you feel that your assignment is performing not as well as expected, you may attempt to switch strategy by setting this option to 'Off'.



Possible values are:



*	On
*	Off
