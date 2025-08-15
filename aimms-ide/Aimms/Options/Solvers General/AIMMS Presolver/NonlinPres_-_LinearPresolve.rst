

.. _Options_NonlinPres_-_LinearPresolve:


Linear Presolve
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether the AIMMS Presolver is called before solving a linear model, a quadratic programming (QP/MIQP) model or a quadratically-constrained programming (QCP/MIQCP) model. Possible values are:



*	On
*	Off




After calling the Presolver AIMMS will pass the presolved model to the solver. A solution obtained from the solver is translated back to the original model but in general sensitivity and basis information will not be complete.





The amount of reductions that the AIMMS Presolver can do is influenced by the options **Presolve Constraints Used** , **Presolve Dual Reductions**  and **Remove Doubletons** , and, in case the model contains binary variables, the option **MINLP Probing** .





**Note** 

*	The option **Nonlinear Presolve**  controls the AIMMS Presolver for nonlinear models.
*	The AIMMS Presolver cannot process constraints that contain an external function and therefore it will ignore such a constraint.
*	The AIMMS Presolver will not be called for models with multi-objectives.
*	The AIMMS Presolver will not be called in case the model is solved using the procedure GMP::SolverSession::AsynchronousExecute.
*	The function GMP::Instance::CreatePresolved will call the AIMMS Presolver underneath and can also be used for linear models.




**Learn more about** 

*	:ref:`Options_NonlinPres_-_MINLP_Probing` 
*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 
*	:ref:`Options_NonlinPres_-_PresolvConstrUsed` 
*	:ref:`Options_NonlinPres_-_Presolve_copy_model` 
*	:ref:`Options_NonlinPres_-_Presolve_Dual_Reductions` 
*	:ref:`Options_NonlinPres_-_Presolve_remove_dupl_vars` 
*	:ref:`Options_NonlinPres_-_RemoveDoubletons` 



