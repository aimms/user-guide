.. _option-GUROBI-nlp_heuristic:


NLP Heuristic
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether Gurobi should use an NLP heuristic to find feasible solutions to non-convex quadratic models and
nonlinear models during a global optimization solve. Possible values are:

    *	Automatic
    *	Off
    *	Moderate
    *	Aggressive
    *	Very aggressive


The NLP heuristic uses a non-linear barrier solver to find feasible solutions to nonconvex quadratic and nonlinear models during a
global optimization solve. It often helps to find solutions quicker, but in some cases it can consume significant runtime without
producing a solution. The value 'Off' disables the heuristic completely, while other values call the heuristic more and more
aggressively during the optimization process.


**Note** 

*	In Gurobi 12.0 and older this option only had possible values 'Yes' (the default) and 'No'.
*	This option only affects non-convex quadratic models and nonlinear models during a global optimization solve.


**Learn more about** 

*	:ref:`option-GUROBI-nonconvex_strategy` 
