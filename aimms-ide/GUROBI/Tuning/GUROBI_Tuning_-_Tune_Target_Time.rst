.. _option-GUROBI-tune_target_time:


Tune Target Time
================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	0.005



This option sets the target runtime in seconds to be reached. As soon as the tuner has found option settings that allow Gurobi to solve the model(s) within the target runtime, it stops trying to improve option settings further. Instead, the tuner switches into the cleanup phase (see the **Tune Cleanup**  option).



**Learn more about** 

*	:ref:`option-GUROBI-tune_cleanup` 
*	:ref:`option-GUROBI-tuning_tool` 
