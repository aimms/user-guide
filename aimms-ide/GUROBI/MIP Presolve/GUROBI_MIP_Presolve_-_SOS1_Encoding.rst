.. _GUROBI_MIP_Presolve_-_SOS1_Encoding:


SOS1 Encoding
=============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option controls the automatic reformulation of SOS1 constraints. Such constraints can be handled directly by the MIP branch-and-cut algorithm, but they are often handled more efficiently by reformulating them using binary or integer variables. There are several different ways to perform this reformulation; they differ in their size and strength. Smaller reformulations add fewer variables and constraints to the model. Stronger reformulations reduce the number of branch-and-cut nodes required to solve the resulting model.



Possible values are:



*	Automatic
*	Multiple choice model
*	Incremental model
*	Logarithmic, emphasize LP relaxation
*	Logarithmic, emphasize branching




Settings 'Multiple choice model' and 'Incremental model' of this option encode an SOS1 constraint using a formulation whose size is linear in the number of SOS members. Setting 'Multiple choice model' uses a so-called multiple choice model. It usually produces an LP relaxation that is easier to solve. Setting 'Incremental model' uses an incremental model. It often gives a stronger representation, reducing the amount of branching required to solve harder problems.





Settings 'Logarithmic, emphasize LP relaxation' and 'Logarithmic, emphasize branching' of this option encode the SOS1 using a formulation of logarithmic size. They both only apply when all the variables in the SOS1 are non-negative. Setting 'Logarithmic, emphasize branching' additionally requires that the sum of the variables in the SOS1 is equal to 1. Logarithmic formulations are often advantageous when the SOS1 constraint has a large number of members. Setting 'Logarithmic, emphasize LP relaxation' focuses on a formulation whose LP relaxation is easier to solve, while setting 'Logarithmic, emphasize branching' has better branching behaviour.





The default value chooses a reformulation for each SOS1 constraint automatically.





**Note** 

*	The reformulation of SOS1 constraints is also influenced by the **SOS1 Reformulation Threshold**  option. To shut off the reformulation entirely you should set that option to 0.




**Learn more about** 

*	:ref:`GUROBI_MIP_Presolve_-_SOS1_Reformulation_Threshold` 
*	:ref:`GUROBI_MIP_Presolve_-_SOS2_Encoding` 



