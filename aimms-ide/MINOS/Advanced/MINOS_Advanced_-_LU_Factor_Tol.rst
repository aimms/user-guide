.. _MINOS_Advanced_-_LU_Factor_Tol:


LU Factor Tolerance
===================



**Type**:	Floating point number	

**Range**:	[1,1e20]	

**Default**:	5	



This option affects the stability and sparsity of the basis factorization B = LU during refactorization. Smaller values for this option favor stability, while larger values favor sparsity. The default value usually strikes a good compromise between stability and sparsity. 



For large and relatively dense problems, 25.0 (say) may give a marked improvement in sparsity without impairing stability to a serious degree.



For certain very special structures (e.g., band matrices) it may be necessary to reduce the value of this option to below 2.0 in order to achieve stability.



**Learn more about** 

*	:ref:`MINOS_Advanced_-_LU_Update_Tolerance`  



