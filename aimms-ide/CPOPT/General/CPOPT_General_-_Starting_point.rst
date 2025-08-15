.. _CPOPT_General_-_Starting_point:


Starting point
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option specifies whether a starting point or solution should be passed to CP Optimizer. Possible values are:



*	Off
*	On




**Note** 

*	By default, AIMMS will pass values for all variables (and activities) to CP Optimizer. By using the procedure GMP::Instance::SetStartingPointSelection it is possible to use only a selection of variables (and activities). 
*	The starting point information is used by the restart and multi-point search types only. It is not used by the depth-first search.




**Learn more about** 

*	:ref:`CPOPT_Search_-_Search_type` 



