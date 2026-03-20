.. _option-ODHCPLEX-maximum_divisor_value:


Maximum Divisor Value
=====================



:Type:	Integer	
:Range:	{1 .. 2100000000}	
:Default:	42



This option sets the maximum divisor value. The model divisor is gradually increased, starting from the **Initial Divisor Value**, until it reaches the value of this option, in which case the ODH engine is terminated. With the **Search Mode**  equal to 'Optimal solution' the solve will continue by the main CPLEX solver; with the **Search Mode**  equal to 'Feasible solution' the solve will terminate.



**Note** 

*	See the section :doc:`../ODH_-_Specifying_Model_Structure` for more information.




**Learn more about** 

*	:doc:`ODH_Advanced_-_Initial_Divisor_Value`  
*	:doc:`../General/ODH_General_-_Search_Mode`  
*	:doc:`../ODH_-_Specifying_Model_Structure` 



