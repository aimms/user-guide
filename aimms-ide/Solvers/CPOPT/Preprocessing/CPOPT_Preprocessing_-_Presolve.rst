.. _option-CPOPT-presolve:


Presolve
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option determines whether table constraints should be preprocessed. Possible values are:



    *	Off
    *	On




CP Optimizer by default presolves the input model before search. Presolve consists in modifying the model to improve it so that it can be solved more efficiently.





Presolve works by


*   simplifying the model by reducing linear constraints by removing redundancies and fixed expressions, and 
*   strengthening the model to achieve more domain reduction by aggregating constraints or factorizing common subexpressions. 




Presolve can be helpful on models that are not well formulated due to the model itself or to the model data.





As a consequence, the overall engine memory consumption can increase because an internal model is created to perform the improvement operations. The presolve transformations are displayed in the output log of CP Optimizer.




