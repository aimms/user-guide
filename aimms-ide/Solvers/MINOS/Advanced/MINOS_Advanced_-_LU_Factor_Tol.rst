.. _option-MINOS-lu_factor_tolerance:


LU Factor Tolerance
===================



:Type:	Floating point number	
:Range:	[1,1e20]	
:Default:	5	



This option affects the stability and sparsity of the basis factorization :math:`B = LU` during refactorization. Smaller values for this
option favor stability, while larger values favor sparsity. The default value usually strikes a good compromise between stability and sparsity. 



For large and relatively dense problems, 25.0 (say) may give a marked improvement in sparsity without impairing stability to a serious degree.



For certain very special structures (e.g., band matrices) it may be necessary to reduce the value of this option to below 2.0 in order to achieve stability.



**Learn more about** 

*	:ref:`option-MINOS-lu_update_tolerance`  



