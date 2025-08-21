.. _CPLEX_Tuning_Tool:


Tuning Tool
===========

The tuning tool looks at options to improve the solving time. If your model suffers from numeric instability, the tuning tool will **not**  attempt to correct that problem. Furthermore, if there is insufficient memory to accommodate optimization of your model, the tuning tool will **not**  correct that problem either. In short, the tuning tool does not magically eliminate all performance bottlenecks. However, if you understand the performance issues of your model, the tuning tool can help you discern option settings that lead to faster solving time.



The tuning tool performs several optimization runs as it goes about its work. These optimization runs may take six to eight times longer than a normal solve. If that projected time seems too long for your purpose, then consider setting a general time limit as controlled by the general solvers option **Time Limit**  or consider setting a specific tuning time limit as controlled by the option **Tuning Time Limit** .



Note that the tuning tool does not return a solution for your model! Also no postsolve or populate will be done.



**Invoking the tuning tool** 

There are two ways to invoke the tuning tool in AIMMS. You can solve a single mathematical program by using the AIMMS routine GMP::Tuning::TuneSingleGMP. For example, to tune a mathematical program 'MP' you should add the following lines to a procedure:



	gmpMP := GMP::Instance::Generate( MP );

    

	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions );



where 'gmpMP' is an element parameter with range 'AllGeneratedMathematicalPrograms' and 'FixedOptions' a subset of AllOptions defining the fixed options (see below).



It is also possible to tune the solver options for a set of MPS or LP problems by using the AIMMS routine GMP::Tuning::TuneMultipleMPS. For example, to tune all '.mps' and '.lp' problems inside a directory 'ProblemSet' use



	GMP::Tuning::TuneMultipleMPS( 'ProblemSet', 'CPLEX 22.1', FixedOptions );



**Tuning tool results** 

The tuned options are always written to the listing file. You can use the optional argument 'ApplyTunedSettings' (default 0) of the tuning procedures, e.g.,



	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions, ApplyTunedSettings : 1 );



to indicate whether the tuned option settings should be used inside the project immediately in which case they become visible in the option tree. Finally, you can use the optional argument 'OptionFileName' of the tuning procedures, e.g.,



	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions, OptionFileName : 'MyOptFile.opt' );



to write out an option file which can be imported into the AIMMS project using the options dialog box.



**Fixed options** 

It is possible to specify a set of options (and their values) that you do not want CPLEX to tune. That is, you want CPLEX to respect those option settings. This is done by the argument 'FixedOptions' in the above mentioned GMP routines. If you pass an empty set for this argument then all options are subject to tuning, even the options that are set to a non-default value inside the AIMMS project!



The general solvers options **MIP Absolute Optimality Tolerance**  and **MIP Relative Optimality Tolerance**  are not subject to tuning. CPLEX will use the option values as specified in the AIMMS project.



CPLEX is equipped with a few options that control the tuning process, e.g., **Tuning Display** , **Tuning Measure**  and **Tuning Repeater** .



**Note** 

*	The tuning tool can be used to tune all type of models including LP.
*	If the tuning tool is used multiple times for the same model then the tuned option settings might vary because the running time of the optimization runs performed by the tuning tool might fluctuate.
*	The tuning tool ignores callbacks specified in AIMMS.




**Learn more about** 

*	:any:`GMP::Tuning::TuneSingleGMP`
*	:any:`GMP::Tuning::TuneMultipleMPS`
*	:ref:`Options_MIP_Options_-_MIP_Absolute_Opt`  
*	:ref:`Options_MIP_Options_-_MIP_Relative_Opt`  
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
*	:ref:`option-CPLEX-tuning_display`  
*	:ref:`option-CPLEX-tuning_measure`  
*	:ref:`option-CPLEX-tuning_repeater`  
*	:ref:`option-CPLEX-tuning_time_limit`  



