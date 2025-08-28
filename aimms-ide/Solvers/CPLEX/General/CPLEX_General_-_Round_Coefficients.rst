.. _option-CPLEX-round_coefficients:


Round Coefficients
==================



:Type:	Floating point number	
:Range:	[0,0.1]	
:Default:	0	



It this option is set to a value larger than 0, matrix coefficients are rounded to the nearest integer value before passing them to CPLEX, if the difference between that integer value and the coefficient is smaller than the value of this option. For example, if the value of a coefficient equals 10.99999999 and the value of this option equals 0.00001 then the coefficient will be rounded to 11. In rare cases using this option can improve the numerical properties of the model and the performance of CPLEX. At the default value of 0, no rounding is done.



Coefficients like 10.99999999 may arise as round-off errors if the matrix coefficients are computed with floating-point arithmetic.



**Note** 

*	Rounding of coefficients close to 0 is controlled by the option **Cleanup C** **oefficients**.




**Learn more about** 

*	:ref:`option-CPLEX-cleanup_coefficients`  
