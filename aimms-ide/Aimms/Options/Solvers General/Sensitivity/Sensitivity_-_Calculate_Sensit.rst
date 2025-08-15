

.. _Options_Sensitivity_-_Calculate_Sensit:


Calculate Sensitivity Ranges
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option determines whether AIMMS will calculate the following sensitivity information for LP or RMIP models:



-	Shadow price ranges for constraints for which the property 'ShadowPriceRange' is set

-	Right hand side ranges for constraints for which the property 'RightHandSideRange' is set

-	Objective coefficient ranges for variables for which the property 'CoefficientRange' is set

-	Value ranges for variables for which the property 'ValueRange' is set



Possible values are:



*	On (Calculate this information)
*	Off (Do not calculate this information)




**Remark** 


The computations required to compute the shadow price ranges or value ranges may considerably increase the total solution time of your mathematical program, because multiple LP problems have to be solved to calculate them. The calculation of the right hand side ranges can also be time consuming.





**Note** 

*	Shadow price ranges and value ranges can be calculated by all linear solvers but right hand side ranges and objective coefficient ranges are only calculated by CPLEX and Gurobi.
*	The option **Time Limit Sensitivity Ranges**  can be used to set a time limit for each LP problem that is solved while calculating shadow price ranges or value ranges.




**Learn more about** 

*	:ref:`Miscellaneous_Calculation_of_Shadow_Price_Ra`  
*	:ref:`Options_Sensitivity_-_Time_Limit_Sensitivity_Ranges`  



