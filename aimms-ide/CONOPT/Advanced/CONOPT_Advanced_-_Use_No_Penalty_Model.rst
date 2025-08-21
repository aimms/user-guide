.. _option-CONOPT-use_no-penalty_model:


Use No-Penalty Model
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option specifies whether CONOPT can use the No-Penalty Model. Possibly values are:



*	Off
*	On




When turned on (the default) CONOPT will create and solve a smaller model without the penalty constraints and variables and the minimax constraints and variables if the remaining constraints are infeasible in the initial point. This is often a faster way to start the solution process.





**Note** 

*	The No-Penalty Model is described in the section :ref:`option-CONOPT-description_of_conopt_algorithm` .




**Learn more about** 

*	:ref:`option-CONOPT-description_of_conopt_algorithm` 



