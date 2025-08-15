

.. _Options_Execution_-_Power_0_0:


Power_0_0
=========



:Type:	Integer	
:Range:	{ -1 .. 1 }	
:Default:	1	



This option controls the result of the operation power(0,0), or, equivalently, 0^0.





*  1 : Then 0^0 is 1, because the lim x ê 0 of x^0 is 1. In addition, this seems to be the predominant choice among software vendors for the operation 0^0. This is the default.
*	0 : Then 0^0 is 0, because the lim x ê 0 of 0^x is 0. In addition, defining 0^0 to be 0 results in more efficient execution as zeros can be skipped.
*	-1 : Then 0^0 is undefined because various choices for this operation can be motivated and in order to avoid any ambiguities during the interpretation of the model such operations should be avoided. This setting is compatible with AIMMS 3 up to AIMMS 3.10.









