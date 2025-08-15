.. _CPLEX_QP_-_MIQCP_Strategy:


MIQCP Strategy
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option sets the strategy that CPLEX uses to solve a quadratically constrained mixed integer program (MIQCP). Possible values are:



*	Automatic
*	Solve QCP relaxations
*	Solve LP relaxations




At the default setting, CPLEX automatically chooses a strategy. When you set this option to the value 'Solve QCP relaxations', you tell CPLEX to solve a QCP node relaxation of the model at each node. When you set this option to the value 'Solve LP relaxations', you tell CPLEX to attempt to solve only an LP node relaxation of the model at each node. 





For some models, the setting 'Solve LP relaxations' may be more effective than 'Solve QCP relaxations'. 




