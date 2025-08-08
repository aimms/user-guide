.. _CPLEX_Troubleshooting:


Troubleshooting
===============

**Out of memory** 

If your model is very large it can happen that there is not enough memory available to solve the model with CPLEX. In case your model contains integer or binary variables you can try to change the option **Node File**  to setting 'On disk' or 'On disk and compressed'.



If CPLEX fails to do a postsolve due to insufficient memory available (while there was enough memory available to do the normal solve) then you might consider to turn off the postsolve by switching off the general solvers option **Postsolve** .



**Ill-conditioned problems** 

Ill-conditioned problems are sensitive to small changes in problem data and tolerance settings (as controlled by options). That is, in such problems, small changes in data or tolerance settings can lead to very large changes in the reported problem solution. CPLEX provides a basis condition number to measure the sensitivity of a linear system to the problem data. You might also think of the basis condition number as the number of places in precision that can be lost. 



For example, if the basis condition number at optimality is 1e+13, then a change in a single matrix coefficient in the thirteenth place (counting from the right) may dramatically alter the solution. Furthermore, since many computers provide about 16 places of accuracy in double precision, only three accurate places are left in such a solution. Even if an answer is obtained, perhaps only the first three significant digits are reliable.



AIMMS will print statistics about the solution quality, including the basis condition number, if the option **Display Solution Statistics**  is switched on.



**Postsolve failure** 

If the postsolve fails then you should switch on the option **Check Solution**  and rerun your AIMMS model. AIMMS will then print additional information in the Message Window. A postsolve failure often indicates that the model is ill-conditioned and poorly scaled.



One particular situation in which the postsolve is likely to fail is if your model contains unscaled infeasibilities. By default, CPLEX scales the model before it is solved (as controlled by the option **Scale** ). CPLEX then tries to find a solution that satisfies the feasibility tolerance with respect to the scaled model. (The feasibility tolerance is controlled by the option **Feasibility** .) Normally, a solution found for the scaled model will also be feasible to the original unscaled model. However, sometimes a solution found by CPLEX might not be feasible to the original model. These unscaled infeasibilities are rare, but they may occur when a problem is ill-conditioned. For example, a problem containing a row in which the coefficients have vastly different magnitude is ill-conditioned in this sense and may result in unscaled infeasibilities.



**Presolver declares model infeasible** 

In case the CPLEX Presolver declares a model as infeasible, the solution reported by CPLEX can usually not be used to analyse where your problem formulation proved infeasible. To get a solution that can be interpreted, you have to rerun your model with the option **Presolve**  turned off or with the option **Preprocessing Reduction Types**  set to an appropriate value.



**Learn more about** 

*	:ref:`Options_Postsolve_-_Postsolve`  
*	:ref:`CPLEX_MIP_-_Node_File`  
*	:ref:`CPLEX_General_-_Check_Solution`  
*	:ref:`CPLEX_General_-_Display_Solution_Statistics`  
*	:ref:`CPLEX_General_-_Scale`  
*	:ref:`CPLEX_Simplex_-_Feasibility` 
*	:ref:`CPLEX_Prepr_-_Presolve`  
*	:ref:`CPLEX_Prepr_-_Pre_reduction_types`  



