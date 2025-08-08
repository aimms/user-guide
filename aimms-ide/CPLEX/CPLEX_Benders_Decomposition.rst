.. _CPLEX_Benders_Decomposition:

Benders Decomposition
=====================

Benders decomposition is a technique that can be used to solve linear programming problems that have a special block structure. This block structure often occurs in applications such as stochastic programming as the uncertainty is usually represented with scenarios. The technique is named after Jacques F. Benders.



In Benders decomposition, the variables of the original problem are divided into two subsets so that a first-stage master problem is solved over the first set of variables, and the values for the second set of variables are determined by solving one or more second-stage subproblems for a given first-stage solution. If one of the subproblems determines that the fixed first-stage decisions are in fact infeasible, then so-called Benders cuts are generated and added to the master problem, which is then re-solved until no cuts can be generated.



The option **Benders Strategy**  should be used to activate the Benders decomposition algorithm in CPLEX. If this option is set to 'Full' then CPLEX will automatically decompose your model. If this option is set to 'User' or 'Worker' then the user must specify a decomposition.



**Specifying a decomposition** 

The user can specify a decomposition by using the AIMMS routine GMP::Column::SetDecomposition. A decomposition value of 0 means that the variable will be assigned to the first-stage master problem. A decomposition value of d >= 1 means that the variable will be assigned to the d-th subproblem (in the second stage).



If the problem contains integer variables then they must become part of the first-stage master problem. If you do not specify a decomposition value for an integer variable then AIMMS will automatically use a decomposition value of 0. Therefore it is not necessary to call the AIMMS routine GMP::Column::SetDecomposition for integer variables. However, you must specify a decomposition value for all continuous variables (except the objective variable).



If your decomposition does not lead to a complete partition of the original model into disjoint master and subproblems, then CPLEX will throw an error. In that case it might be helpful to look at the detailed information printed by AIMMS, as controlled by the option **Benders Decomposition Check Limit** .



**Limitations** 

CPLEX only supports Benders decomposition for linear problems. CPLEX does not support Benders decomposition for problems with ranged, indicator, SOS or lazy constraints. Benders decomposition is also not supported for multi-objective optimization problems.



The Benders decomposition algorithm supports the incumbent, iterations and time callback procedures, but only for MIP problems. The branch, candidate, cut, heuristic, lazy constraint and status change callback procedures are not supported.



A solve of an LP or RMIP problem in which CPLEX is using the Benders decomposition algorithm cannot be interrupted.



The Progress Window is not updated if CPLEX uses the Benders decomposition algorithm to solve an LP or RMIP problem. (The Progress Window is updated if an MIP problem is solved.)



**Note** 

*	The Benders strategies 'User' and 'Worker' require you to use GMP functionality. The Benders strategy 'Full' can also be applied to a normal solve-statement.
*	AIMMS itself contains an Automatic Benders’ Decomposition module which can be used in combination with any linear solver. The AIMMS Automatic Benders algorithm does not support multiple subproblems.




**References** 

*	J. Benders. Partitioning procedures for solving mixed-variables programming problems, Numerische Mathematik, volume **4** , issue 1, pages 238–252, 1962.
*	M. Fischetti, D. Salvagnin, A. Zanette. A note on the selection of Benders’ cuts, Mathematical Programming, series B, volume **124** , pages 175-182, 2010.
*	M. Fischetti, I. Ljubic, M. Sinnl. Benders decomposition without separability: a computational study for capacitated facility location problems, Technical Report University of Padova, 2016.




**Learn more about** 

*	:ref:`CPLEX_Benders_-_Benders_Strategy` 
*	:ref:`CPLEX_Benders_-_Benders_Decomposition_Check_Limit` 
*	:any:`GMP::Column::SetDecomposition`



