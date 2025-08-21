.. _option-GUROBI-disconnected_component_strategy:


Disconnected Component Strategy
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



A MIP model can sometimes be made up of multiple, completely independent sub-models. This option controls how aggressively Gurobi tries to exploit this structure. Possible values are:



*	Automatic
*	Off
*	Moderate
*	Aggressive




Setting 'Off' ignores this structure entirely. At the default value Gurobi chooses automatically.




