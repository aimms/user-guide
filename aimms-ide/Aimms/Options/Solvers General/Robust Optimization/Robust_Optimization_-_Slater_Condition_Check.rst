

.. _Options_Robust_Optimization_-_Slater_Condition_Check:


Slater Condition Check
======================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	On	



This option determines whether AIMMS checks the regularity conditions for the uncertainty set. To do so, AIMMS formulates a problem to find a point in the interior of the uncertainty set. If this model is infeasible then this implies that uncertainty set is empty and generation of the robust counterpart (using the function GMP::Instance::GenerateRobustCounterpart) will fail. If the model is feasible but there exists no point in the interior of the uncertainty set, then the regularity conditions are not satisfied and AIMMS will generate a warning. As a consequence, the robust counterpart might become numerical instable and the solver might face difficulties solving it, especially if the robust counterpart is a second-order cone program (SOCP).



**Warning: You should only switch off this option if you are certain that the uncertainty set is not empty. If you switch off this option while the uncertainty set is empty, the robust counterpart generated can be feasible but the solution returned will be meaningless!** 



Possible values are:



*	On
*	Off




**Note** 

*	If the model contains ellipsoidal uncertainty constraints then the problem for checking the regularity conditions will be a second-order cone program, as will be the robust counterpart. Otherwise it will be a linear program.
*	AIMMS can print the constraint listing of the uncertain mathematical program by setting the option **Constraint Listing Robust Optimization**  to 'Uncertain mathematical program' or 'Both'.




**Learn more about** 

*	:ref:`Options_Robust_Optimization_-_Constraint_Listing_RO` 
*	:ref:`Options_Robust_Optimization_-_Slater_Condition_Tolerance`  






