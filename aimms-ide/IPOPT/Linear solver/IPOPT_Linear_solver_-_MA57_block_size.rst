

.. _option-IPOPT-ma57_block_size:


MA57 block size
===============



:Type:	Integer	
:Range:	{1..2147483647}	
:Default:	16	



This option controls the block size used by Level 3 BLAS in MA57BD.


**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA57'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
