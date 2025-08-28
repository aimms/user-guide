.. _option-KNITRO-multistart_termination_condition:


Multistart Termination Condition
================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Normal	



This option specifies the condition for terminating multistart. Possible values are:



    *	Normal
    *	First optimal solution
    *	First feasible solution
    *	Any
    *	Rule based




With the default setting the multistart algorithm terminates if the number of start points tried equals the value as specified with the option **Number of Multistart Points** .





With the setting 'First optimal solution' the multistart algorithm terminates if the value of **Number of Multistart Points**  is exceeded or after the first local optimal solution is found (whichever comes first).





With the setting 'First feasible solution' the multistart algorithm terminates if the value of **Number of Multistart Points**  is exceeded or after the first feasible solution estimate is found (whichever comes first).





With the setting 'Any' the multistart algorithm terminates if the value of **Number of Multistart Points**  is exceeded or after the first solution estimate of any type is found (whichever comes first).


 


With the setting 'Rule based' the multistart algorithm terminates using rules that estimate when the probability of finding new local solutions is low.





This option has only effect if the option **Multistart**  is switched on.





**Learn more about** 

*	:ref:`option-KNITRO-multistart`  
*	:ref:`option-KNITRO-number_of_multistart_points`  
