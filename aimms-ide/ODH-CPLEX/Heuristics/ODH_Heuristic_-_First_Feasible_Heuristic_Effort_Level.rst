.. _option-ODHCPLEX-first_feasible_heuristic_effort_level:


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

*	:ref:`option-ODHCPLEX-first_feasible_heuristic`  
*	:ref:`option-ODHCPLEX-search_mode`  
