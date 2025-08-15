

.. _Options_Interface_-_Solver_Input_Preci:


Solver Input Precision
======================



:Type:	Integer	
:Range:	{0..15}	
:Default:	0	



This option determines how input values for the solvers are truncated by AIMMS. The truncation is such that the first Solver Input Precision digits of the input values are passed to the solver, whereas the remaining digits are set to a unique value. When this option is set to 0, there will be no truncation.



The exact rule for truncation is quite complicated. A double is stored as 8 bytes (64 bits in modern computers) in computer memory and the truncation procedure changes some of the bits. As a result a "nice" value as 262.9 might become an "ugly" value as 262.89999999999418 (if solver input precision equals 13). In fact all values in the interval [262.89999999997963, 262.90000000000867] will be translated into this value.



Numbers that are almost equal will often be projected onto the same value (if the solver input precision is sufficiently large) but in some cases they might be projected onto different values that are relatively far from each other.



**Note** 

*	This an advanced option. If you set this option to a non-default value there is a risk of unexpected or incorrect behavior in your application.
*	 You should never set the value of this option to a value below 13 (except 0).



