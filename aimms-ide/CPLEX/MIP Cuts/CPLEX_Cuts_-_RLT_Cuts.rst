.. _CPLEX_Cuts_-_RLT_Cuts:


RLT Cuts
========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option controls the addition of cuts based on the Reformulation Linearization Technique (RLT) for nonconvex quadratic programs (QP) or mixed integer quadratic programs (MIQP) solved to global optimality, that is, if the option **Solution Target**  is set to 'Search for global optimum'. Possible values are:



*	Off
*	Automatic
*	Generate cuts moderately
*	Generate cuts aggressively
*	Generate cuts very aggressively




**Note** 

*	CPLEX does not apply BQP cuts to mixed integer linear programs (MIP).




**Learn more about** 

*	:ref:`CPLEX_QP_-_Solution_Target` 




**References** 

*	H. D. Sherali and W. P. Adams, A Reformulation-Linearization Technique for Solving Discrete and Continuous Nonconvex Problems, Springer, 1999.
