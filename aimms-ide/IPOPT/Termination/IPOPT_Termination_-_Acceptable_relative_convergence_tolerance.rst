

.. _option-IPOPT-acceptable_relative_convergence_tolerance:


Acceptable relative convergence tolerance
=========================================



:Type:	Floating point number	
:Range:	[1e-010,1e+019]	
:Default:	1e-006	



This option determines which (scaled) overall optimality error is considered to be "acceptable." There are two levels of termination criteria. If the usual "desired" tolerances (see the options **Relative Convergence Tolerance** , **Dual Infeasibility Tolerance** , etc) are satisfied at an iteration, the algorithm immediately terminates with a success message. On the other hand, if the algorithm encounters a certain number of iterations in a row that are considered "acceptable" and this number equals to value of the option **Maximum Number of Acceptable Iterations** , it will terminate before the desired convergence tolerance is met. This is useful in cases where the algorithm might not be able to achieve the "desired" level of accuracy.



**Learn more about** 

*	:ref:`option-IPOPT-dual_infeasibility_tolerance` 
*	:ref:`option-IPOPT-maximum_number_of_acceptable_iterations` 
*	:ref:`option-IPOPT-relative_convergence_tolerance` 
