

.. _Advanced_-_LU_Update_Tolerance:
.. _MINOS_Advanced_-_LU_Update_Tolerance:


LU Update Tolerance
===================



**Type**:	Floating point number	

**Range**:	[1,1e20]

**Default**:	5	



This option affects the stability and sparsity of the basis factorization B = LU during updating. Smaller values for this option favor stability, while larger values favor sparsity. The default value usually strikes a good compromise between stability and sparsity. 



For large and relatively dense problems, 25.0 (say) may give a marked improvement in sparsity without impairing stability to a serious degree.



**Learn more about** 

*	:ref:`MINOS_Advanced_-_LU_Factor_Tol`  



