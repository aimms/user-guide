

.. _option-IPOPT-relative_convergence_tolerance:


Relative convergence tolerance
==============================



:Type:	Floating point number	
:Range:	[1e-010,1e+019]	
:Default:	1e-008	



This option determines the convergence tolerance for the algorithm. The algorithm terminates successfully, if the (scaled) NLP error becomes smaller than this value, and if the (absolute) criteria according to the options **Dual Infeasibility Tolerance**  and **Complementarity Tolerance**  are met. See also the option **Acceptable Relative Convergence Tolerance**  as a second termination criterion. Note, some other algorithmic features also use this quantity to determine thresholds etc.



**Learn more about** 

*	:ref:`option-IPOPT-acceptable_relative_convergence_tolerance` 
*	:ref:`option-IPOPT-complementarity_tolerance` 
*	:ref:`option-IPOPT-dual_infeasibility_tolerance` 
