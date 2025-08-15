

.. _Options_Feasibility_relaxation:


Feasibility Relaxation
======================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Standard	



This option determines which feasibility relaxation to use. If the option is set to 'Standard', AIMMS will use the built-in method of handling violation penalties. If this option is set to 'Advanced', AIMMS will use FeasOpt (if CPLEX is used) or FeasRelax (if Gurobi is used). If the option is set to 'Advanced', but neither CPLEX nor Gurobi is selected as solver, AIMMS will default to the standard approach. 



If violation penalties are specified for the optimization model, AIMMS will automatically generate excess variables for the specified constraints. In the built-in approach, AIMMS will add a penalty term - for each excess variable - to the original objective. In contrast, if FeasOpt or FeasRelax is used, a minimum cost relaxation is calculated. The objective for this minimum cost relaxation can be set using the option **Feasibility Relaxation Objective** . Optionally, one can choose to optimize the original objective among the solutions that have a minimum cost relaxation. This can be set using the option **Feasibility Relaxation Optimize Original Objective** . 



Possible values are:



*	Standard
*	Advanced




**Note** 

*	This option is only relevant if violation penalties are specified for the model. 
*	If this option is set to 'Advanced', callbacks specified in AIMMS are ignored. 
*	The AIMMS approach of handling violation penalties allows the user to specify the keyword 'zero' when defining the violation penalties. If 'zero' is specified, AIMMS will add the violation variable, but it will not create the corresponding term in the objective. In contrast, FeasOpt and FeasRelax cannot handle a value of 'zero' for the violation penalties.




**Learn more about** 

*	`Infeasibility analysis <https://documentation.aimms.com/language-reference/optimization-modeling-components/solving-mathematical-programs/infeasibility-analysis.html>`_ (Language Reference) 
*	:ref:`Options_Feasibility_relaxation_objecti`  
*	:ref:`Options_Feasibility_relaxation_optimiz`  
*	:ref:`CPLEX_Feasibility_Relaxation`  
*	:ref:`GUROBI_FeasRelax_Feasibility_Relaxation`  



