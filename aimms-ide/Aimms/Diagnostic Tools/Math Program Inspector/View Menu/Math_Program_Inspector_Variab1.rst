

.. _Diagnostic-Tools_Math_Program_Inspector_Variab1:


Variable Solution
=================

**Description** 

By selecting Variable Solution from the View menu, the Variable Solution tab is opened. As soon as a solution is available, this tab reveals more details about this solution. The Variable Solution tab shows the following seven columns:



*	Variable,
*	Lower Bound,
*	Value (i.e. solution/level value),
*	Upper Bound,
*	Marginal (i.e. reduced cost),
*	Basis Status (i.e. Basic or Nonbasic), and
*	Bound Status (i.e. At bound, In between bounds, or Bound violation).




By clicking in the header of a column you can sort the table according to that specific column.





**Note** 


The information for marginals and basis statuses is retrieved from the solver. This information cannot be retrieved if you solve two models, and open the Math Program Inspector for the first model, because the first model will no longer be loaded in the solver (only the second model). To have AIMMS store this information for the first model you should switch on the following options:




*	:ref:`option-AIMMS-always_store_basics`  (for basis statuses)
*	:ref:`option-AIMMS-always_store_marginals`  (for marginals)




Instead of setting these options you can also switch on the option :ref:`option-AIMMS-store_complete_solver_solution`.





(In case GMP functionality is used to solve the models then the first model will remain loaded in the solver, unless the GMP corresponding to the first model is deleted, and in that case there is no need to set these options.)




