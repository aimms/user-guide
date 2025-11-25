

.. _option-AIMMS-infeasibility_finder_postsolve:


Infeasibility Finder Postsolve
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



If this option is switched 'On' and the LP model solved during the postsolve turns out to be infeasible, then the irreducible infeasibility set (IIS)
will be written to the listing file. Analyzing this IIS can help with improving the robustness of the model. Possible values are:

    *	On
    *	Off


**Note** 

*	By default AIMMS will suppress the writing of the IIS for encrypted AIMMS projects; see the option **Suppress Listing File Encrypted Project**.
*	This option can be used by the following solvers: :ref:`SolverCPLEX`, :ref:`SolverGurobi` and :ref:`SolverCOPT`.
*	CPLEX will use its conflict refiner if this option is switched on to construct an irreducible infeasibility set (IIS).
*	This option was added in AIMMS 25.9.1.


**Learn more about** 

*	:ref:`option-AIMMS-postsolve`  
*	:ref:`option-AIMMS-suppress_listing_file_encrypted_project` 

