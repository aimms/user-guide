.. _option-GUROBI-tune_output_level:


Tune Output Level
=================



:Type: 	Integer
:Range: 	{0 .. 3}
:Default: 	2



This option controls the amount of output produced by the tuning tool.



Level 0 produces no output.

Level 1 produces tuning summary output only when a new best option set is found.

Level 2 produces tuning summary output for each option set that is tried.

Level 3 produces tuning summary output, plus detailed solver output, for each option set tried.



**Note** 

*	Output by the tuning tool is not written to the output file if the option **Output File**  is switched off.
*	If this option is set to 0 or 1 then the 'Tuning Progress' in the Progress Window will not be updated.
*	Gurobi output uses 'parameter' instead of 'option'.




**Learn more about** 

*	:ref:`option-GUROBI-output_file` 
*	:ref:`option-GUROBI-tuning_tool` 
