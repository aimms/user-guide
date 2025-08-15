.. _CPLEX_General_-_NumericalEmphasis:


Numerical Emphasis
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option lets you indicate to CPLEX that it should emphasize precision in numerically difficult or unstable problems, with consequent performance trade-offs in time and memory. Possible values are:



*	No
*	Yes




**Note** 

*	With numerical emphasis switched on, CPLEX will apply extra precaution, and will examine solutions with more care than as usual. This can result in more solutions being rejected.
