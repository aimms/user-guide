.. _CBC_MIP_Heur_-_Greedy_heuristic:


Greedy heuristic
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option determines whether to use the greedy heuristic. Setting 'On' switches on the greedy heuristic (after preprocessing) which will try and obtain a solution. It may just fix a percentage of variables and then try a small branch-and-cut run.



Setting 'Before' means that the greedy heuristic is used before preprocessing if option **Heuristics**  is switched on, off otherwise. Setting 'Both' means that the greedy heuristic is used before preprocessing if option **Heuristics**  is switched on, and during the solve. Possible values are:



*	Off
*	On
*	Before
*	Both




**Learn more about** 

*	:ref:`CBC_MIP_Heur_-_Heuristics`  
