.. _KNITRO_General_-_Linear_Solver:


Linear Solver
=============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option indicates which linear solver Knitro should use to solve linear systems arising in Knitro algorithms. Possible values are:



*	Automatic
*	Hybrid
*	QR
*	MA27
*	MA57
*	MKL PARDISO




For setting 'Hybrid' the solver is chosen depending on the particular linear system which needs to be solved. Setting 'QR' uses a dense QR method. This approach uses LAPACK QR routines. Since it uses a dense method, it is only efficient for small problems. It may often be the most efficient method for small problems with dense Jacobians or Hessian matrices. Settings 'MA27' and 'MA57' use to corresponding HSL sparse symmetric indefinite solver. Setting 'MKL PARDISO' activates the Intel MKL PARDISO sparse symmetric indefinite solver.





The Intel MKL PARDISO solver can run in parallel by using the option **Number of Linear System Threads** . It can run out-of-core by using the option **Linear Solver Out of Core** .





**Learn more about** 

*	:ref:`KNITRO_General_-_Linear_Solver_Node_Amalgamation` 
*	:ref:`KNITRO_General_-_Linear_Solver_Ordering` 
*	:ref:`KNITRO_General_-_Linear_Solver_Out_of_Core` 
*	:ref:`KNITRO_General_-_Linear_Solver_Scaling` 
*	:ref:`KNITRO_Par_-_Number_of_Lin_Sys_Threads`  



