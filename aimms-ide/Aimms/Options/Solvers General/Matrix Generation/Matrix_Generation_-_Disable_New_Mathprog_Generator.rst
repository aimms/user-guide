

.. _option-AIMMS-disable_new_mathprog_generator:


Disable New Mathprog Generator
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



In AIMMS 24.6 a new implementation for the generation of a mathematical program has been introduced. This implementation is not yet complete with respect to all the features that may be present in a mathematical program. By default, the new generator will attempt to generate the model, but only for LP and MIP models. If the new generator fails for some reason, the generation stops and falls back to the old way of generating. You will get warning messages containing the reason(s) why the generation was not done by the new generator. If there is not an easy way to work around the unsupported feature(s) it is better to not let the new generation try, and thus just rely on the old generation. Setting this option to 'On' will disable the new generator.



Possible values are:



*	On
*	Off




Currently, the old generator will always be used if:




*	For a mathematical program that is not an LP or MIP.
*	For generating a robust or stochastic model via the GMP functions: GMP::Instance::GenerateRobustCounterpart or GMP::Instance::GenerateStochasticProgram.
*	If one of the constraint or variable definitions contains a (rare) expression that is not yet supported by the new compiler.



