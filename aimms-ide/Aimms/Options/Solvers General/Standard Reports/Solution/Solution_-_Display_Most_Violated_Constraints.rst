

.. _option-AIMMS-display_most_violated_constraints_and_bounds:


Display Most Violated Constraints and Bounds
============================================



:Type:	Integer	
:Range:	{-1 .. :ref:`Miscellaneous_Maxint`}	
:Default:	0	



This option controls whether or not to display information about the largest constraint violations, bound violations and integer violations in the constraint listing. 

If this option is unequal to 0, a summary table will be printed, which contains:

    *	the largest constraint violation, the sum of constraint violations and the number of constraint violations;
    *	the largest variable bound violation, the sum of variable bound violations and the number of variable bound violations;
    *	the largest integrality violation, the sum of integrality violations and the number of integrality violations (only for models that contain integer variables).


Additionally, if this option equals :math:`n > 0`, the :math:`n` largest constraint violations, variable bound violations
and integer violations are printed, provided that these violations are larger than the value of the option
**Constraint Listing Feasibility Tolerance**.


**Note** 

*	By default AIMMS will suppress the writing of the largest constraint violations, variable bound violations and integer violations for encrypted AIMMS projects; see the option **Suppress Listing File Encrypted Project**. This option does not suppress the printing of the summary table. 
*	This option is only used for linear models. For non-linear models, the information will not be printed to the listing file. 


**Learn more about** 

*	:ref:`option-AIMMS-constraint_listing_feasibility_tolerances` 
*	:ref:`option-AIMMS-suppress_listing_file_encrypted_project` 

