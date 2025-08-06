.. _GUROBI_Presolve_-_Presolve_Dual:


Presolve Dual
=============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option controls controls whether presolve forms the dual of a continuous model. Depending on the structure of the model, solving the dual can reduce overall solution time. The default setting uses a heuristic to decide. Setting 'Off' forbids presolve from forming the dual, while setting 'Force' forces it to take the dual. Setting 'Presolve primal and dual' employs a more expensive heuristic that forms both the presolved primal and dual models (on two threads), and heuristically chooses one of them. Possible values are:



*	Automatic
*	Off
*	Force
*	Presolve primal and dual



