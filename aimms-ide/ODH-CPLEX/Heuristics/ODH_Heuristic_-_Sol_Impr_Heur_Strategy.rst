.. _option-ODHCPLEX-solution_improvement_heuristic_strategy:


Solution Improvement Heuristic Strategy
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Moderate	



This option specifies the solution improvement heuristic strategy. Possible values are:



*	Normal
*	Moderate
*	Aggressive




The aggressive strategy setting attempts to make more progress with each sub-model solve at the cost of more expensive sub solves. Amongst other changes, it sets **Initial Divisor Value** , **Maximum Divisor Repeats**  and **Maximum Divisor Value**  if they are not explicitly set by the user.





**Learn more about** 

*	:ref:`option-ODHCPLEX-initial_divisor_value`  
*	:ref:`option-ODHCPLEX-maximum_divisor_repeats`  
*	:ref:`option-ODHCPLEX-maximum_divisor_value`  
