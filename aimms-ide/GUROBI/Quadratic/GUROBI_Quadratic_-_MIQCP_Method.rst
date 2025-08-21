.. _option-GUROBI-miqcp_method:


MIQCP Method
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls the method used to solve MIQCP models. Value 'Linearizations' uses a linearized, outer-approximation approach, while value 'QCP relaxations' solves continuous QCP relaxations at each node. The default setting chooses automatically. Possible values are:



*	Automatic
*	Linearizations
*	QCP relaxations



