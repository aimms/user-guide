.. _CPLEX_General_-_Farkas_Infeasibility_Proof:


Farkas Infeasibility Proof
==========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



This option specifies whether CPLEX should retrieve a Farkas infeasibility proof once CPLEX detects that the model is infeasible. Possible values of this option are:



*	No
*	Yes




Assume the values returned for the constraints are stored in an array y[] which has the following interpretation. For the i-th constraint, if that constraint is a less-than-or-equal-to constraint, y[i] <= 0 holds; if that constraint is a greater-than-or-equal-to constraint, y[i] >= 0 holds. Thus, where b is the right-hand-side vector for the given linear program, A is the constraint matrix, and x denotes the vector of variables, y may be used to derive the following valid inequality:





	yTA x >= yTb





Here y is being interpreted as a column vector, and yT denotes the transpose of y. The real point of computing y is the following. Suppose we define a vector z of dimension equal to the dimension of x and having the following value for entries





	zj = uj	where yTAj > 0, and 


	zj = lj	 where yTAj < 0,





where Aj  denotes the column of A corresponding to xj, uj the given upper bound on xj, and lj is the specified lower bound. (zj is arbitrary if yTAj = 0.) Then y and z will satisfy





	yTb - yTA z > 0.





This last inequality contradicts the validity of yTA x >= yTb, and hence shows that the given linear program is infeasible.





The constraint values in the Farkas infeasibility proof are passed to AIMMS instead of the normal level values for the constraints. Note that the general solvers option **Always Store Constraint Levels**  should be switched on.





The quantity yTb - yTA z in some sense denotes the degree of infeasibility. It is stored in the .SumOfInfeasibilities suffix of the math program.





**Note** 

*	The Farkas infeasibility proof is only available for LP and RMIP models.
*	If the presolver detects infeasibility (or indicates that the model is InfeasibleOrUnbounded) then the Farkas infeasibility proof is not available. In that case, turn **Presolve**  off and reoptimize to obtain the Farkas infeasibility proof.
*	If you are using the barrier optimizer without crossover (see the option **LP Method** ) then the Farkas infeasibility proof is not available. 




**Learn more about** 

*	:ref:`Options_Sensitivity_-_Always_Store_Con`  
*	:ref:`CPLEX_General_-_LP_Method`  
*	:ref:`CPLEX_Prepr_-_Presolve`  
