

.. _Options_Matrix_Generation-Mathematical_Program_Type_Check:


Mathematical Program Type Check
===============================



:Type:	Selection
:Range:	The settings listed below
:Default:	Post Generation



The type of a mathematical program is verified when specified by the model developer or determined by AIMMS. This option specifies at which moment the type of a mathematical program is actually determined or verified.



Any inconsistencies in the type of a mathematical program as specified by the model builder and as determined by AIMMS, should be reported as early as possible. However, when the sets of variables or constraints, as given in the attributes "variables" or "constraints" of a mathematical program, may change at run time, it does not make sense to check the type of a mathematical program at compile time. Moreover, when the sets and parameters referenced in the index domain conditions of variables and constraints may change, thereby potentially changing the type of the generated mathematical program, it only makes sense to check the type at the end of the generation.



Possible values are:



*	Compile Time - The type of a mathematical program is determined or verified at compile time; runtime changes in the set of variables or constraints cannot be taken into account but inconsistencies detected in the type of the mathematical program are reported before any computations are done.
*	Pre Generation - The type of a mathematical program is determined or verified at the start of generating that mathematical program; runtime changes in the set of variables and constraints are taken into account, but the contents of identifiers restricting the generation of variables and constraints are not taken into account. Inconsistencies detected in the type of the mathematical program are reported before the actual generation, but after the determination of the data used to instantiate the mathematical program.
*	Post Generation - The type of a mathematical program is determined or verified after it is generated. Both runtime changes in the set of variables and the set of constraints determining the mathematical programs as well as the data used to instantiate the mathematical program are taken into account. Inconsistencies detected in the type of the mathematical program are reported only after the mathematical program is generated.



