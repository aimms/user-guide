.. _option-CBC-crash:


Crash
=====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether to create a basis for the problem. If crash is switched on and there is an all slack basis then CBC will flip or put structural variables into the basis with the aim of getting dual feasible. On the whole dual seems to be better without it. Possible values are:



*	Off
*	On
*	Solow-Halim
*	Modified Solow-Halim




**Learn more about** 

*	:ref:`option-CBC-idiot_crash`  
