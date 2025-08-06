.. _CPLEX_MIP_Advanced_-_Write_Cuts_Variable_Val:


Write Cuts Variable Values
==========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Off	



This option determines whether a list of cuts and constraints should be followed by a list of variables referenced in that cut or constraint. Such a list contains for each variable its lower bound, its level value and its upper bound. Possible values are:



*	Off
*	On




This option can only be used in combination with the options **Find Fractional Root Solution**  and **Write Cuts** .





The level values correspond to the fractional solution found at the end of the root node. The lower and upper bounds correspond to the bounds in the presolved model (of CPLEX).





**Note** 

*	If this option is switched on then also the left-hand-side of all cuts and constraints will be evaluated and printed.




**Learn more about** 

*	:ref:`CPLEX_MIP_Advanced_-_Find_Fractional_Root_Solution` 
*	:ref:`CPLEX_MIP_Advanced_-_Write_Cuts` 
