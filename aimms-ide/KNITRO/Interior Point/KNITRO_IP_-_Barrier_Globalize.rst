.. _KNITRO_IP_-_Barrier_Globalize:


Barrier Globalize
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Filter	



This option specifies the globalization strategy used by the interior-point algorithms. Possible values are:



*	None
*	Karush-Kuhn-Tucker
*	Filter




With the setting 'None', Knitro does not apply a globalization strategy.





With the setting 'Karush-Kuhn-Tucker', a globalization strategy based on decreasing the KKT error is applied.





With the default setting 'Filter', a globalization strategy using a filter based on the objective and constraint violation is applied.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 



