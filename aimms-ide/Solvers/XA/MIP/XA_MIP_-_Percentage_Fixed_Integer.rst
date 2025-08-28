.. _option-XA-percentage_fixed_integer_variables:


Percentage Fixed Integer Variables
==================================



:Type:	Real	
:Range:	[0,100]	
:Default:	0.0	



This option determines the percentage of available integer variables that are fixed at each integer node. The default value of 0.0 means no fixing. Adjusting this value can be useful for very large binary problems. If 100.0 is entered then all integer columns that are integer at the end of solving the relaxed LP problem are fixed at the current integer bounds.



