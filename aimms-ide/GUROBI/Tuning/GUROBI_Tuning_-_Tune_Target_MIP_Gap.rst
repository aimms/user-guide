.. _option-GUROBI-tune_target_mip_gap:


Tune Target MIP Gap
===================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	0.005



This option sets a target MIP gap to be reached. As soon as the tuner has found option settings that allow Gurobi to reach the target MIP gap for the given model(s), it stops trying to improve option settings further. Instead, the tuner switches into the cleanup phase (see the **Tune Cleanup**  option).



**Learn more about** 

*	:ref:`option-GUROBI-tune_cleanup` 
*	:ref:`option-GUROBI-tuning_tool` 
