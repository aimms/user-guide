

.. _option-MINOS-feasibility_tolerance:


Feasibility Tolerance
=====================



:Type:	Floating point number	
:Range:	[1e-15,1000]	
:Default:	1e-6	



MINOS tries to ensure that all variables eventually satisfy their upper and lower bounds to within the absolute tolerance defined by the value of this option. This includes slack variables. Hence, the general constraints are also satisfied to within the feasibility tolerance.



MINOS attempts to find a feasible point before optimizing the objective function. If the sum of infeasibilities cannot be reduced to zero, the problem is declared infeasible. If the sum of infeasibilities is quite small, it may be appropriate to raise the feasibility tolerance by a factor 10 or 100. Otherwise, some error in the data should be suspected.



Note: if the sum of infeasibilities is not small, there may be other points that have a significantly smaller sum of infeasibilities. MINOS does not attempt to find the solution that minimizes the sum of infeasibilities.



If scaling is used (i.e., the value of the option **Scale Method**  is not equal to 'No scaling'), feasibility is defined in terms of the scaled problem (since it is then more likely to be meaningful).



A nonlinear objective function F(x) will be evaluated only at feasible points. If there are regions where F(x) is undefined, every attempt should be made to eleminate these regions from the problem. For example, if F(x) = Öx1 + log(x2), it is essential to place lower bounds on both variables x1 and x2. If the feasibility tolerance equals 1e-6, the bounds x1 >= 1e-5 and x2 >= 1e-4 might be appropriate. (The log singularity is more serious. In general, keep x as far away from singularities as possible.)



Bounds should also be used to keep x more than t (the value of this option) away from singularities in other nonlinear functions f(x).



If there are any nonlinear constraints, each major oteration attemps to satisfy their linearization to within the feasibility tolerance. If this is not possible, the bounds on the nonlinear constraints are relaxed temporarily (in several stages).



Feasibility with respect to the nonlinear constraints themselves is measured against the **Row Tolerance**  (not againts the feasibility tolerance). The relevant test is made at the start of a major iteration.



**Learn more about** 

*	:ref:`option-MINOS-row_tolerance`  
*	:ref:`option-MINOS-scale_method`  



