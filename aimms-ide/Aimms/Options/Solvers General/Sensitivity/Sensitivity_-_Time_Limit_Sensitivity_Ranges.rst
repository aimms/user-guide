

.. _Options_Sensitivity_-_Time_Limit_Sensitivity_Ranges:


Time Limit Sensitivity Ranges
=============================



**Type**:	Integer	

**Range**:	{0..:ref:`Miscellaneous_Maxint`  }	

**Default**:	:ref:`Miscellaneous_Maxint` 	



This option specifies a time limit (in CPU seconds) for each LP problem that is solved while calculating shadow price ranges or (variable) value ranges.



**Note** 

*	If the solver hits the time limit while solving such an LP problem, then the corresponding smallest or largest shadow price/variable value is assigned the value UNDF (undefined).




**Learn more about** 

*	:ref:`Options_Sensitivity_-_Calculate_Sensit`  
*	:ref:`Miscellaneous_Calculation_of_Shadow_Price_Ra`  



