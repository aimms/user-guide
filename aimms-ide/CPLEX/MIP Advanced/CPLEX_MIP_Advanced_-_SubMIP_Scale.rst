.. _option-CPLEX-submip_scale:


SubMIP Scale
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Standard	



This option decides how to scale the problem matrix when CPLEX solves a subMIP during MIP optimization. Possible values are:



*	None (no scaling)
*	Standard (use equilibration scaling)
*	Aggressive (use aggressive scaling)




SubMIPS are described in the section :ref:`option-CPLEX-submip` .





**Note** 

*	This rarely used option is helpful **only**  in rare "corner" cases where there is clear evidence that the default scaling value is really inappropriate for this particular problem.




**Learn more about** 

*	:ref:`option-CPLEX-submip` 
