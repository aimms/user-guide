.. _KNITRO_Term_-_Objective_Goal:


Objective Goal
==============



**Type** :	Floating point number	

**Range** :	[-1e20,1e20]	

**Default** :	1e20	



This option is used to implement a custom stopping condition based on the objective function value. Knitro will stop and declare that a satisfactory solution was found if a feasible objective function value at least as good as the value specified by this option is achieved. This stopping condition is only active when the absolute value of this option is less than 1e20.



