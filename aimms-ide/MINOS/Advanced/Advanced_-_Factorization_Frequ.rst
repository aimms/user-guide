

.. _Advanced_-_Factorization_Frequ:
.. _MINOS_Advanced_-_Factorization_Frequ:


Factorization Frequency
=======================



:Type:	Integer	
:Range:	{1..10000000}	
:Default:	50	



This option determines how many basis changes at most will occur between factorizations of the basis matrix.



With linear programs, the basis factors are usually updated every iteration. The default value of 50 is reasonable for typical problems. Higher values up to 100 (say) may be more efficient on problems that are extremely sparse and well scaled. 



When the objective function is nonlinear, fewer basis updates will occur as an optimum is approached. The number of iterations between basis factorizations will therefore increase. During these iterations a test is made regularly (according to the value of the option **Check Frequency** ) to ensure that the general constraints are satisfied. If necessary the basis will be refactorized before the limit, as defined by the value of this option, is reached.



When the constraints are nonlinear, the **Maximum Number of Minor Iterations**  limit will probably preempy this option.



**Learn more about** 

*	:ref:`MINOS_Advanced_-_Check_Frequen` 
*	:ref:`MINOS_-_Maximum_Number_of_Min` 

 




