.. _option-SNOPT-factorization_frequency:


Factorization Frequency
=======================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	50	



This option determines how many basis changes at most will occur between factorizations of the basis matrix.



With linear programs, the basis factors are usually updated every iteration. The default value of 50 is reasonable for typical problems. Higher values up to 100 (say) may be more efficient on problems that are extremely sparse and well scaled. 



When the objective function is nonlinear, fewer basis updates will occur as an optimum is approached. The number of iterations between basis factorizations will therefore increase. During these iterations a test is made regularly (according to the value of the option **Check Frequency** ) to ensure that the general constraints are satisfied. If necessary the basis will be refactorized before the limit, as defined by the value of this option, is reached.



**Learn more about** 

*	:ref:`option-SNOPT-check_frequency`  

 




