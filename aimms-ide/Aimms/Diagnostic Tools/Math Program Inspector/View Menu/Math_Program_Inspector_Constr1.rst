

.. _Diagnostic-Tools_Math_Program_Inspector_Constr1:


Constraint Solution
===================

**Description** 

By selecting Constraint Solution from the View menu, the Constraint Solution tab is opened. As soon as a solution is available, this tab reveals more details about this solution. The Constraint Solution tab shows the following five columns:



*	Constraint,
*	Value (i.e. solution),
*	Marginal (i.e. shadow price),
*	Basis Status (i.e. Basic or Nonbasic), and
*	Bound Status (i.e. Binding, Nonbinding, or Violated).




By clicking in the header of a column you can sort the table according to that specific column.





**Note** 


The information for values, marginals, basis statuses and bound statuses is retrieved from the solver. This information cannot be retrieved if you solve two models, and open the Math Program Inspector for the first model, because the first model will no longer be loaded in the solver (only the second model). To have AIMMS store this information for the first model you should switch on the following options:




*	:ref:`option-AIMMS-always_store_basics`  (for basis statuses)
*	:ref:`option-AIMMS-always_store_constraint_levels`  (for values and bound statuses)
*	:ref:`option-AIMMS-always_store_marginals`  (for marginals)




Instead of setting these options you can also switch on the option :ref:`option-AIMMS-store_complete_solver_solution`.





(In case GMP functionality is used to solve the models then the first model will remain loaded in the solver, unless the GMP corresponding to the first model is deleted, and in that case there is no need to set these options.)




