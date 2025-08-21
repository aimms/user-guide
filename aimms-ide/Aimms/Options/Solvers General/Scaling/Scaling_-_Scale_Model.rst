

.. _Options_Scaling_-_Scale_Model:


Scale Model
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether AIMMS should scale the model before sending it to the solver. Possible values are:



*	On
*	Off




After scaling the model, AIMMS will pass the scaled model to the solver. Solutions obtained from the solver are translated back to the original model.





The scaling algorithm used by AIMMS is controlled by the option **Scaling Algorithm** . The option**List Scaling Factors**  can be used to list the scaling factors, as found by the scaling algorithm, that are used in the scaled model. The option **Constraint Listing Scaled Model**  can be activated to use the scaled model and solution for printing the constraint listing.





In case the same model is solved multiple times, possibly with small modifications, then the model will not be scaled again, and the scaling factors of the first solve will be applied to the consecutive solves. Any (GMP) modifications in the model will be scaled according to these scaling factors, of course.





Scaling is not supported for:




*	Constraint programming models,
*	Models with complementarity constraints,
*	GMP's generated using GMP::Instance::CreateDual,
*	GMP's generated using GMP::Instance::GenerateRobustCounterpart, and
*	GMP's generated using GMP::Instance::GenerateStochasticProgram.




A model can also be scaled by using the :ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model`  in the Math Program Inspector but the scaling is then only done inside the Math Program Inspector which means that the scaling factors are not automatically applied to the model, that is, you have to change the Unit attribute of the variables and constraints to incorporate the scaling factors.





One of the advantages of using this option is that AIMMS automatically applies all scaling factors underneath, so you do not have to change your model.





AIMMS keeps track of a scaling score which, more or less, measures how well the model is scaled. The score is calculated by using the variable bounds, the right-hand-side values of the constraints, and the matrix coefficients of each couple of variable and constraint. For each of these terms the largest and smallest value (in absolute sense) is determined. If the largest value lv is larger than 1 then this term contributes to the scaling score by power(10,ceil(log10(lv))), that is, we round up lv to the next 10 power. If the smallest value sv is smaller than 1 then this term contributes to the scaling score by power(10,ceil(-log10(sv))). A lower score corresponds to a better scaled model.





For example, if the constraint c1(i) has right-hand-side values 200, 20, 10 and 0.01 then the contribution of this constraint is 1000 + 100 = 1100. Without the 0.01 value the contribution would have been 1000.





Infinite variable bounds, and variable bounds and right-hand-side values equal to 0 are not scaled. They also do not contribute to the scaling score.





AIMMS reports the scaling score before and after scaling the model. If the Combination algorithm is used then AIMMS will also report the scaling score after the first step.





**Note** 

*	The scaling factors will be powers of 10.
*	Most solvers have implemented their own scaling algorithm(s). The corresponding solver specific options that control their scaling algorithm(s) have been listed in the section below.




**Learn more about** 

*	:ref:`Options_Scaling_-_Constraint_Listing_Scaled_Model` 
*	:ref:`Options_Scaling_-_List_Scaling_Factors` 
*	:ref:`Options_Scaling_-_Scaling_Algorithm` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model` 
*	:ref:`option-CBC-scaling`
*	:ref:`option-CONOPT-scaling_method`
*	:ref:`option-COPT-scale`
*	:ref:`CPLEX_General_-_Scale`
*	:ref:`GUROBI_General_-_Scale`
*	:ref:`KNITRO_General_-_Scaling`
*	:ref:`SNOPT_Scaling_-_Scale_Method`





