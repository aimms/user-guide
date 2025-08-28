.. _option-CPLEX-cut_limit:


Cut Limit
=========



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	2100000000	



This option sets a limit for each type of cut. This option allows you to set a uniform limit on the number of cuts of a each type that CPLEX generates. There is no effective limit by default. Tighter limits on the number of cuts of each type may benefit certain models. For example, a limit on each type of cut will prevent any one type of cut from being created in such large number that the limit on the total number of all types of cuts is reached before other types of cuts have an opportunity to be created.



A setting of 0 means no cuts.



**Note** 

*	This option does not influence the number of Gomory cuts.




**Learn more about** 

*	:ref:`option-CPLEX-gomory_cuts`  



