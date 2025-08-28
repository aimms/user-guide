

.. _Diagnostic-Tools_Math_Program_Inspector_Constra:


Constraint Statistics
=====================

**Description** 

By selecting Constraint Statistics from the View menu, the Constraint Statistics tab is opened. 
This tab displays information about the current constraint selection. 
Most of the statistics that are displayed on this tab are self explanatory. 
Two cases may need additional explanation. In case a single symbolic (first-level node) has been selected, 
the Index domain density statistic will display the number of actually generated constraints as a percentage of the full domain (i.e. the domain without any domain condition applied). 
In case a single constraint (a leaf node) has been selected, the statistics 
will be extended with some specific information about the constraint, 
such as rhs-values and solution values (e.g. level value and shadow price).

The number of infeasible constraints reported takes into account the option **MPI Feasibility Tolerance**. 
This tolerance is not used for calculating the maximum and total constraint violation. 
Therefore it can happen that the number of infeasible constraints equals 0 while the maximum and total constraint violation are unequal to 0. 
Setting the **MPI Feasibility Tolerance**  to 0 resolves this discrepancy.

**Note that** 

*   When a single symbolic constraint has been selected, the lower part of the constraint statistics tab displays the symbolic form of the constraint definition.
*   When a single constraint is selected (a leaf node), the lower part of the constraint statistics tab contains also a list with associated variables, the coefficients of these variables in the constraint, their values and their primal contributions.

**Note** 

The information for level values, shadow prices, basis statuses and bound statuses is retrieved from the solver. This information cannot be retrieved if you solve two models, and open the Math Program Inspector for the first model, because the first model will no longer be loaded in the solver (only the second model). To have AIMMS store this information for the first model you should switch on the following options:

*   :ref:`option-AIMMS-always_store_basics`  (for basis statuses)
*   :ref:`option-AIMMS-always_store_constraint_levels`  (for level values and bound statuses)
*   :ref:`option-AIMMS-always_store_marginals`  (for shadow prices)

Instead of setting these options you can also switch on the option :ref:`option-AIMMS-store_complete_solver_solution`.

(In case GMP functionality is used to solve the models then the first model will remain loaded in the solver, unless the GMP corresponding to the first model is deleted, and in that case there is no need to set these options.)

**Learn more about** 

*   :ref:`chap:mpinspector`
*   :ref:`option-AIMMS-mpi_feasibility_tolerance`  



