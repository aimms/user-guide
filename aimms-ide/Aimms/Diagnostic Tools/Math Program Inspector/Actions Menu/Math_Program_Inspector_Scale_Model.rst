.. _Diagnostic-Tools_Math_Program_Inspector_Scale_Model:

Scale Model
===========

**Description** 

The Scale Model action from the Actions menu can be used to find scaling factors 
for the symbolic variables and constraints in a linear model which can be used to 
improve the numerical properties of the model, 
possibly resulting in more accurate solutions or performance improvements. 
Note that solvers like CPLEX, Gurobi and COPT also use algorithms to scale 
the model but in our experience it often helps to use units or scaling factors 
in the AIMMS model to improve the numerical properties of the model.

If this action is selected then AIMMS will solve a MIP model to find the scaling factors. 
The size of the MIP model is usually fairly small as it is limited 
by the number of symbolic variables and constraints in the original model. 
The scaling tool will try to scale the variables and constraint in such a way that all coefficients,
right-hand-side values and variable bounds will become as close to 1 (in absolute sense) as possible. 
In other words, it will try to reduce the number of red blocks in the :ref:`Diagnostic-Tools_Math_Program_Inspector_Matrix1` . 
Note, however, that binary and integer variables will not be scaled.

By switching on the option **Scale Using Solution**  the scaling tool will use the current solution 
(if any) in the Math Program Inspector to scale the model. The focus then (partially) 
shifts from making the Matrix View green to getting a solution in which 
the variables get level values close to 1 (in absolute sense).

Once the scaling tool is finished, a new tab :ref:`Diagnostic-Tools_Math_Program_Inspector_Scaling_Factors`  
will be opened containing the scaling factors for all variables and constraints in the model. 
You can now select the :ref:`Diagnostic-Tools_Math_Program_Inspector_Resolve` action from 
the Actions menu to resolve the model which will then use the new scaling factors. 
If using these new scaling factors seems to help solving your model then you can decide 
to apply these scaling factors in your model which means adjusting the Unit attribute of 
the variables and constraints. 
Please note that if you select a variable or constraint in the Scaling Factors tab, 
you can use right-mouse-click to open the attributes window of the corresponding variable or constraint.

The scaling factors can be printed in the listing file by setting the option **List Scaling Factors**  to 'Automatic' or 'Symbolic'.

The Scale Model action is only available for linear models and it is not supported for:

*	GMP's generated using GMP::Instance::CreateDual,
*	GMP's generated using GMP::Instance::GenerateRobustCounterpart,
*	GMP's generated using GMP::Instance::GenerateStochasticProgram, and
*	GMP's generated using GMP::Instance::CreatePresolved.

A model can also be scaled, outside the Math Program Inspector, by activating the **Scale Model**  option. 
The main advantage of using this option is that AIMMS automatically applies all scaling factors underneath, 
so you do not have to change your model. 
Another advantage is that it can be used to scale a nonlinear model.

**Note** 

*	The scaling factors will be powers of 10.

**Learn more about** 

*	:ref:`Options_Scaling_-_List_Scaling_Factors` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Matrix1` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Resolve` 
*	:ref:`Options_Scaling_-_Scale_Model` 
*	:ref:`Options_Math_Program_Inspector_-_Scale_using_Solution` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scaling_Factors` 
*   :ref:`sec:units.ident`

*	:ref:`sec:units.ident`



