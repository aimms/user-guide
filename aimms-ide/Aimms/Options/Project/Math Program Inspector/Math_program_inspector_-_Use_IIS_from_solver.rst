

.. _option-AIMMS-use_iis_from_solver:


Use IIS From Solver
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option determines whether an Irreducible Inconsistent System will be retrieved directly from the solver if the action Irreducible Inconsistent System (IIS) is selected in the Math Program Inspector. Possible values are:



    *	No
    *	Yes




If this option is set to 'Yes' then AIMMS will let the solver calculate the Irreducible Inconsistent System (IIS for short) using an algorithm implemented in the solver. If this option is set to 'No' then the IIS is calculated using an algorithm implemented in AIMMS (which involves solving several subproblems using a solver).





Advantages of letting the solver calculate the IIS are:




*	It is faster.
*	For models with integer variables it also finds an IIS if the infeasibility is triggered by the integrality of some of the variables.
*	It can be used for models with indicator constraints.
*	It can be used for quadratic models (QP, MIQP, QCP, MIQCP) solved by CPLEX or Gurobi, and for QP models solved by COPT.




Letting the solver calculate the IIS has one minor disadvantage, namely in some cases it requires that the action Resolve must be selected in the Math Program Inspector before the action Irreducible Inconsistent System (IIS) becomes available. This is the case if:




*	The model has been modified inside the Math Program Inspector, and the action Substructure Causing Infeasibility is selected first.
*	A second model is solved after solving the first model (and no GMP functionality is used), and the Math Program Inspector is opened for the first model.




**Note** 

*	The IIS calculated by the AIMMS' algorithm calculates the IIS for the relaxed model in which the integer variables are made continuous. If this relaxed model is feasible then the IIS will not be available.
*	The algorithm for calculating the IIS and implemented in AIMMS is described in The User’s Guide.
*	The solver CBC cannot calculate an IIS itself. Therefore the AIMMS' algorithm will always be used for CBC even if this option is set to 'Yes'.
*	For an infeasible model, the IIS calculated by the solver will be the same as the one which is calculated if the option **Infeasibility Finder**  is switched on.




**Learn more about** 

*	:ref:`aimmshelp26-Math_Program_Inspector` 
*	:ref:`option-AIMMS-infeasibility_finder` 
