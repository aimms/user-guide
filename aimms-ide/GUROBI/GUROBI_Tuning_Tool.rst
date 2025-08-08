.. _GUROBI_Tuning_Tool:


Tuning Tool
===========

Gurobi provides a wide variety of options that allow you to control the operation of the optimization engines. The level of control varies from extremely coarse-grained to very fine-grained. While these options provide a tremendous amount of user control, the immense space of possible options can present a significant challenge when you are searching for option settings that improve performance on a particular model. The purpose of the Gurobi tuning tool is to automate this search.



The Gurobi tuning tool performs multiple solves on your model, choosing different option settings for each, in a search for settings that improve runtime. The longer you let it run, the more likely it is to find a significant improvement. The option **Tune Time Limit**  can be used to control the amount of time spent searching for an improving option set.



While option settings can have a big performance effect for many models, they aren't going to solve every performance issue. One reason is simply that there are many models for which even the best possible choice of option settings won't produce an acceptable result. Some models are simply too large and/or difficult to solve, while others may have numerical issues that can't be fixed with option changes.



Another limitation of automated tuning is that performance on a model can experience significant variations due to random effects (particularly for MIP models). This is the nature of search. The Gurobi algorithms often have to choose from among multiple, equally appealing alternatives. Seemingly innocuous changes to the model (such as changing the order of the constraint or variables), or subtle changes to the algorithm (such as modifying the random number seed) can lead to different choices. Often times, breaking a single tie in a different way can lead to an entirely different search. We've seen cases where subtle changes in the search produce 100X performance swings. While the tuning tool tries to limit the impact of these effects, the final result will typically still be heavily influenced by such issues.



The bottom line is that automated performance tuning is meant to give suggestions for options that could produce consistent, reliable improvements on your models. It is not meant to be a replacement for efficient modeling or careful performance testing.



Note that the tuning tool does not return a solution for your model! Also no postsolve will be done.



**Invoking the tuning tool** 

There are two ways to invoke the tuning tool in AIMMS. You can solve a single mathematical program by using the AIMMS routine GMP::Tuning::TuneSingleGMP. For example, to tune a mathematical program 'MP' you should add the following lines to a procedure:



	gmpMP := GMP::Instance::Generate( MP );

    

	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions );



where 'gmpMP' is an element parameter with range 'AllGeneratedMathematicalPrograms' and 'FixedOptions' a subset of AllOptions defining the fixed options (but not used by Gurobi; see below).



It is also possible to tune the solver options for a set of MPS or LP problems by using the AIMMS routine GMP::Tuning::TuneMultipleMPS. For example, to tune all '.mps' and '.lp' problems inside a directory 'ProblemSet' use



	GMP::Tuning::TuneMultipleMPS( 'ProblemSet', 'GUROBI 12.0', FixedOptions );



**Tuning tool results** 

The tuned options are always written to the listing file. You can use the optional argument 'ApplyTunedSettings' (default 0) of the tuning procedures, e.g.,



	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions, ApplyTunedSettings : 1 );



to indicate whether the tuned option settings should be used inside the project immediately in which case they become visible in the option tree. Finally, you can use the optional argument 'OptionFileName' of the tuning procedures, e.g.,



	GMP::Tuning::TuneSingleGMP( gmpMP, FixedOptions, OptionFileName : 'MyOptFile.opt' );



to write out an option file which can be imported into the AIMMS project using the options dialog box.



**Fixed options** 

Options that have been set to a non-default value inside the AIMMS project will not be subject to tuning. The only exception is the option **Method**  which will always be tuned. The 'FixedOptions' argument in the GMP procedures above is not used by Gurobi.



Gurobi is equipped with a few options that control the tuning process, e.g., **Tune Cleanup** , **Tune Criterion** , **Tune Results** , **Tune Time Limit** , **Tune Trials Tune**  and **Output Level** .



**Note** 

*	The tuning tool can be used to tune all type of models including LP.
*	If the tuning tool is used multiple times for the same model then the tuned option settings might vary because the running time of the optimization runs performed by the tuning tool might fluctuate.
*	The tuning tool ignores callbacks specified in AIMMS.




**Learn more about** 

*	:any:`GMP::Tuning::TuneSingleGMP`
*	:any:`GMP::Tuning::TuneMultipleMPS`
*	:ref:`GUROBI_Tuning_-_Tune_Cleanup` 
*	:ref:`GUROBI_Tuning_-_Tune_Criterion` 
*	:ref:`GUROBI_Tuning_-_Tune_Metric` 
*	:ref:`GUROBI_Logging_-_Tune_Output_Level` 
*	:ref:`GUROBI_Tuning_-_Tune_Results` 
*	:ref:`GUROBI_Tuning_-_Tune_Target_MIP_Gap` 
*	:ref:`GUROBI_Tuning_-_Tune_Target_Time` 
*	:ref:`GUROBI_Tuning_-_Tune_Time_Limit` 
*	:ref:`GUROBI_Tuning_-_Tune_Trials` 
