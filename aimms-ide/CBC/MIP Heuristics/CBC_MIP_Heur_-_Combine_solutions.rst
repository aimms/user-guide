.. _option-CBC-combine_solutions:


Combine solutions
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off



This option determines whether to use the combine solutions heuristic. Setting 'On' switches on a heuristic (after preprocessing) which does branch-and-cut on the problem given by just using variables which have appeared in one or more solutions. It is obviously only tried after two or more solutions.



Setting 'Before' means that the combine solutions heuristic is used before preprocessing if option **Heuristics**  is switched on, off otherwise. Setting 'Both' means that the combine solutions heuristic is used before preprocessing if option **Heuristics**  is switched on, and during the solve. Possible values are:



*	Off
*	On
*	Before
*	Both




**Learn more about** 

*	:ref:`option-CBC-heuristics`  
