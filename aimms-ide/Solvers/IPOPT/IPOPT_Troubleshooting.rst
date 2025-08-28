.. _IPOPT_Troubleshooting:


Troubleshooting
===============

**IPOPT does not solve model** 

If IPOPT does not solve the model then you should enable printing of the status file by switching on the option **Status File**. The status file usually contains useful information explaining why IPOPT could not solve the model.



Some reasons that IPOPT cannot solve a model are:




*   Problem has too few degrees of freedom. IPOPT first checks whether the number of (unfixed) variables is greater-or-equal than the number of equality constraints. If this is not the case then IPOPT will regard the problem as over-constrained and stop with this message. (This conclusion is based on assumptions on constrained qualifications, basically, that there are no redundant equality constraints.) To resolve this issue you should try to reduce the number of equality constraints in the model. You could also try to switch on the general solvers option **Nonlinear Presolve**  which could possibly remove redundant




*   Restoration Failed. This indicates that the restoration phase failed to find a feasible point that was acceptable to the filter line search for the original problem. This can happen if the problem is highly degenerate or does not satisfy the constraint qualification.



**Learn more about** 

*	:ref:`option-AIMMS-nonlinear_presolve` 
*	:ref:`option-IPOPT-status_file` 
