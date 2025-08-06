.. _CBC_MIP_Heur_-_Rounding_heuristic:


Rounding heuristic
==================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	On	



This option determines whether to use the rounding heuristic. Setting 'On' switches on a simple (but effective) rounding heuristic at each node of the tree (after preprocessing). Setting 'Before' means that the rounding heuristic is used before preprocessing if option **Heuristics**  is switched on, off otherwise. Setting 'Both' means that the rounding heuristic is used before preprocessing if option **Heuristics**  is switched on, and during the solve.



Possible values are:



*	Off
*	On
*	Before
*	Both




**Learn more about** 

*	:ref:`CBC_MIP_Heur_-_Heuristics`  
