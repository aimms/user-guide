

.. _option-IPOPT-ma57_small_pivot_parameter:


MA57 small pivot parameter
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



If this option is switched on, then when small entries are detected by the linear solver MA57 they are removed and the corresponding pivots are placed at the end of the factorization. This can be particularly efficient if the matrix is highly rank deficient. Possible values are:



*	Off
*	On




**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA57'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
