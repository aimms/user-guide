.. _CPLEX_General_-_Cleanup_Coefficients:


Cleanup Coefficients
====================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0	



CPLEX will change matrix coefficients that are smaller in magnitude than the value of this option to 0. This practice is also known as zero-ing out the negligible coefficients, and it is done just before the actual solve starts. Such coefficients may arise as round-off errors if the matrix coefficients are computed with floating-point arithmetic. At the default value of 0, no cleanup is done.



**Learn more about** 

*	:ref:`CPLEX_General_-_Round_Coefficients`  
