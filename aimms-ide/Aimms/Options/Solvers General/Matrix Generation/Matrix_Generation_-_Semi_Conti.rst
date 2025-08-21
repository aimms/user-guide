

.. _option-AIMMS-semi_continuous_max_bound:


Semi Continuous Max Bound
=========================



:Type:	Floating point number	
:Range:	[100, 1.0e80]	
:Default:	1.0e8	



When semi continuous variables have large bounds, there is a risk of numerical instability. With this option you can specify a bound. Whenever an absolute bound of a column in a semi continuous variable is larger than the setting of this option, the AIMMS matrix generator will return an error message.





