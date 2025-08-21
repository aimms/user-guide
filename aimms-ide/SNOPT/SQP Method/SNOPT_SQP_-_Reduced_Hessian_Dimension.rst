.. _option-SNOPT-reduced_hessian_dimension:


Reduced Hessian Dimension
=========================



:Type:	Integer	
:Range:	{-1..1000000}	
:Default:	-1	



This option specifies that an i × i triangular matrix R is to be available for use by the QP Cholesky solver (to define the reduced Hessian according to RTR = ZTHZ). The value of i affects when QP solver CG is activated.



The default value of -1 is special; in that case the reduced Hessian dimension is set equal to the number of nonlinear variables plus 1 (but will never be larger than 2000).



**Learn more about** 

*	:ref:`option-SNOPT-qp_solver`  
