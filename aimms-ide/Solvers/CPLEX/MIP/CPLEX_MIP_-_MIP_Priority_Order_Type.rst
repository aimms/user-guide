.. _option-CPLEX-mip_priority_order_type:


MIP Priority Order Type
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option selects the type of generic priority order to generate. Possible values are:

    *	Off
    *	Decreasing cost
    *	Increasing bound range
    *	Increasing cost per coefficient count


This option will only be active if the option **MIP Priority Order Switch** is switched on, and if no ``Priority`` attribute
of a variable is specified in the AIMMS project.


**Learn more about** 

*	:doc:`CPLEX_MIP_-_MIP_Priority_Order_Switch <CPLEX_MIP_-_MIP_Priority_Order_Switch>` 
