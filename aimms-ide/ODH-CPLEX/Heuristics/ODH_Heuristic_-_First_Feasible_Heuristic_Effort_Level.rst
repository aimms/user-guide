.. _ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic_Effort_Level:


First Feasible Heuristic Effort Level
=====================================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	500	



This option specifies the effort limit on the **First Feasible Heuristic**  for finding an initial feasible solution. Values are:



>0 = use this level of effort

<0 = use no more than -X effort, where X is the value of this option



The larger the effort level, the more effort is expended before giving up.



**Note** 

*	This option is only used if the **Search Mode**  equals 'Feasible solution'.




**Learn more about** 

*	:ref:`ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic`  
*	:ref:`ODH-CPLEX_General_-_Search_Mode`  
