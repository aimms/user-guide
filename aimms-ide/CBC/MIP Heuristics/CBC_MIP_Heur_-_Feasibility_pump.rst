.. _option-CBC-feasibility_pump:


Feasibility pump
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option determines whether to use the Feasibility Pump heuristic. This is due to Fischetti and Lodi and uses a sequence of LPs to try and get an integer feasible solution. Some fine tuning is available by the option **Feasibility Pump Passes** .



With setting 'On' the Feasibility Pump heuristic is used after preprocessing. Setting 'Before' means that the Feasibility Pump heuristic is used before preprocessing if option **Heuristics**  is switched on, off otherwise. Setting 'Both' means that the Feasibility Pump heuristic is used before preprocessing if option **Heuristics**  is switched on, and during the solve. Possible values are:



*	Off
*	On
*	Before
*	Both




**Learn more about** 

*	:ref:`option-CBC-feasibility_pump_passes`  
*	:ref:`option-CBC-heuristics`  
