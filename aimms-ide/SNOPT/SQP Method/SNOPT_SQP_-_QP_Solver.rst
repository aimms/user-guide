.. _SNOPT_SQP_-_QP_Solver:


QP Solver
=========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Cholesky	



This option specifies the method used to solve the reduced Hessian system for the search directions in phase 2 of the QP subproblem. Possible values are:



*	Cholesky
*	CG
*	QN




The Cholesky solver holds the full Cholesky factor R of the reduced Hessian ZTHZ. As the minor iterations proceed, the dimension of R changes with the number of superbasic variables. If the number of superbasic variables needs to increase beyond the value of the Reduced Hessian dimension, the reduced Hessian cannot be stored and the solver switches to the CG solver. The Cholesky solver is reactivated if the number of superbasics stabilizes at a value less than the Reduced Hessian dimension.





The QN solver solves the QP using a quasi-Newton method similar to that of MINOS. In this case, R is the factor of a quasi-Newton approximate Hessian.





The CG solver uses an active-set method similar to the QN solver, but uses the conjugate-gradient method to solve all systems involving the reduced Hessian.





The Cholesky solver is the most robust, but may require a significant amount of computation if the number of superbasics is large.





The quasi-Newton solver does not require the computation of the R at the start of each QP subproblem. It may be appropriate when the number of superbasics is large but relatively few major iterations are needed to reach a solution (e.g., if SNOPT is called with a good starting point).





The conjugate-gradient solver is appropriate for problems with large numbers of degrees of freedom (say, more than 2000 superbasics).





**Learn more about** 

*	:ref:`SNOPT_SQP_-_Reduced_Hessian_Dimension`  
