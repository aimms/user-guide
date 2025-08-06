.. _GUROBI_Quadratic_-_MIQCP_Formulation:


MIQCP Formulation
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option specifies the format of the presolved MIQCP model. This option only affects MIQCP models. Possible values are:



*	Automatic
*	MIQCP
*	MISOCP
*	Disaggregated MISOCP




Setting 'MIQCP' leaves the model in MIQCP form, so the branch-and-cut algorithm will operate on a model with arbitrary quadratic constraints.





Setting 'MISOCP' always transforms the model into MISOCP form; quadratic constraints are transformed into second-order cone constraints.





Setting 'Disaggregated MISOCP' always transforms the model into disaggregated MISOCP form; quadratic constraints are transformed into rotated cone constraints, where each rotated cone contains two terms and involves only three variables.





The default setting chooses automatically. The automatic setting works well, but there are cases where forcing a different form can be beneficial.




