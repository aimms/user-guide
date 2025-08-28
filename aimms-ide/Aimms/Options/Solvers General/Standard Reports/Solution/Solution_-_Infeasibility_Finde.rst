

.. _option-AIMMS-infeasibility_finder:


Infeasibility Finder
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



If this option is switched 'On' and a model is infeasible, extra information will be written to the listing file. Possible values are:



    *	On
    *	Off




**Note** 

*	By default AIMMS will suppress the writing of the irreducible infeasibility set (IIS) for encrypted AIMMS projects; see the option **Suppress Listing File Encrypted Project**.
*	The following solvers have an infeasibility finder: CPLEX, Gurobi, COPT, CONOPT and BARON.
*	The infeasibility finder can also be used for infeasible MIP models using CPLEX, Gurobi or COPT, or nonlinear models using Gurobi.
*	CPLEX will use its conflict refiner if this option is switched on to construct an irreducible infeasibility set (IIS).
*	XA's infeasibility finder will only be used if this option is switched on and the XA option **Force**  is set to 'Yes'.
*	CONOPT's infeasibility finder only finds infeasibilities in recursive and triangular equations.
*	BARON's infeasibility finder will only be used if this option is switched on and the BARON option **Compute IIS**  is set to a non-default value.
*	An alternative for locating infeasibilities in your model is available via the violation penalty attribute of the mathematical program.




**Learn more about** 

*	:ref:`option-Baron-compute_iis`
*	:ref:`option-XA-force` 
*	:ref:`Model-Explorer_Creating_a_Mathematical_Progra`  
*	:ref:`option-AIMMS-suppress_listing_file_encrypted_project` 



