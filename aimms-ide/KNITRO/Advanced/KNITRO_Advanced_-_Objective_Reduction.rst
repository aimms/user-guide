.. _KNITRO_Advanced_-_Objective_Reduction:


Objective Reduction
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option indicates whether or not objective reduction should be used before passing a model to Knitro. Possible values are:



*	Off
*	On




By default, if a model contains an objective variable then AIMMS will try to remove that variable from the model. For example, assume we have a model containing objective variable 'obj' with a constraint





	obj = 2*x1 + 3*x2





then with objective reduction AIMMS will remove 'obj' and the above constraint from the model, and pass '2*x1 + 3*x2' as the objective function to Knitro. Without objective reduction, 'obj' will be passed as the objective function and the above constraint will be passed as a (regular) constraint to Knitro.





Note that objective reduction is not possible if the objective variable is part of more than one constraint (or variable definition).




