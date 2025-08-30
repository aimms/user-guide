.. _option-SNOPT-lu_update_tolerance:


LU Update Tolerance
===================



:Type:	Floating point number	
:Range:	[1,1e20] + {na}	
:Default:	na	



This option affects the stability and sparsity of the basis factorization B = LU during updating. Smaller values for this option favor stability, while larger values favor sparsity. The default value usually strikes a good compromise. 



The default value of this option depends on the model class of the problem. For LP models it is 10.0 and for NLP it is 3.99.



For certain very regular structures (e.g., band matrices) it may be necessary to reduce the value of this option (and that of option **LU Factor Tolerance**) in order to achieve stability.



**Learn more about** 

*	:ref:`option-SNOPT-lu_factor_tolerance`  



