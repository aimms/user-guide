

.. _Baron_Variable_Priorities:


Variable Priorities
===================

BARON implements branch-and-bound algorithms involving convex relaxations of the original problem. Branching takes place not only on integer variables, but also on continuous variables that are nonlinear. Users can specify branching priorities for both integer and continuous variables.



To specify variable branching priorities, you can use the Priority attribute or the .Priority suffix of a variable; see the Language Reference. The priority value has to be nonnegative. All variables with priority 0 (zero) will be considered last by BARON. For variables with a positive priority value, those with the highest priority value will be considered first.



**Remark** 

The rule for transforming AIMMS priority values to BARON priority values is as follows:



  BARON priority = AIMMS priority + 1



**Note** 

*	Only variables with an AIMMS priority value unequal to 0 (corresponding to a BARON priority value of 1) are written to the BRANCHING_PRIORITIES section of the model file (see option **Keep model file**).




**Learn more about** 

*	:ref:`option-Baron-keep_model_file` 
