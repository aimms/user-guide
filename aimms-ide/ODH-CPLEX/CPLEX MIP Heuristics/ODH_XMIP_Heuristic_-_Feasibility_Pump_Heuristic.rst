.. _ODH-CPLEX_XMIP_Heuristic_-_Feasibility_Pump_Heuristic:


Feasibility Pump Heuristic
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option is used to turns on or off the feasibility pump heuristic. Possible values are:



*	Off
*	Automatic
*	Emphasis feasible solution
*	Emphasis good solution




At the default setting, CPLEX automatically chooses whether or not to apply the feasibility pump heuristic on the basis of characteristics of the model.





To turn on the feasibility pump heuristic regardless of characteristics of the model, set the option to 'Emphasis feasible solution' or 'Emphasis good solution'. If the option is set to 'Emphasis feasible solution', the feasibility pump tries to find a feasible solution without taking the objective function into account. If the option is set to 'Emphasis good solution', the heuristic usually finds solutions of better objective value, but is more likely to fail to find a feasible solution.





For more detail about the feasibility pump heuristic, see research by Fischetti, Glover, and Lodi (2003, 2005), by Bertacco, Fischetti, and Lodi (2005), and by Achterberg and Berthold (2005, 2007). 





**Note** 

*	Branching priorities have no effect on the feasibility pump heuristic.
