

.. _Diagnostic-Tools_Math_Program_Inspector_Variabl:


Variable Statistics
===================

**Description** 

By selecting Variable Statistics from the View menu, the Variable Statistics tab is opened. This tab displays information about the current variable selection. Most of the statistics that are displayed on this tab are self explanatory. Two cases may need additional explanation. In case a single symbolic (first-level node) has been selected, the Index domain density statistic will display the number of actually generated variables as a percentage of the full domain (i.e. the domain without any domain condition applied). In case a single variable (a leaf node) has been selected, the statistics will be extended with some specific information about the variable such as bound values and solution values (e.g. level value and reduced cost).



**Note that** 

*	When a single variable has been selected (a leaf node) the lower part of the variable statistics tab contains a list with the associated constraints, the coefficients of the selected variable in those constraints and their corresponding shadow prices and dual contributions.




**Note** 


The information for reduced costs and basis statuses is retrieved from the solver. This information cannot be retrieved if you solve two models, and open the Math Program Inspector for the first model, because the first model will no longer be loaded in the solver (only the second model). To have AIMMS store this information for the first model you should switch on the following options:




*	:ref:`option-AIMMS-always_store_basics`  (for basis statuses)
*	:ref:`option-AIMMS-always_store_marginals`  (for reduced costs)




Instead of setting these options you can also switch on the option :ref:`option-AIMMS-store_complete_solver_solution`.





(In case GMP functionality is used to solve the models then the first model will remain loaded in the solver, unless the GMP corresponding to the first model is deleted, and in that case there is no need to set these options.)





**Learn more about** 

*   :ref:`chap:mpinspector`



