.. _option-ODHCPLEX-mip_priority_order_switch:


MIP Priority Order Switch
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option decides whether to use the priority order, if one exists, for the next mixed integer optimization. Possible values are:



*	Off
*	On




A priority order can be specified in two ways, namely (1) by specifying a branching priority in the AIMMS project using the Priority attribute of a variable, or (2) by setting the option **MIP Priority Order Type**  to a non-default value. If you switch off this option then the priority order specified by either way will be ignored.





**Note** 

*	If the Priority attribute of a variable is specified in the AIMMS project then the option **MIP Priority Order Type**  will be switched off.




**Learn more about** 

*	:ref:`option-ODHCPLEX-mip_priority_order_type` 
