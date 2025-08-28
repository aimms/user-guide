.. _option-SNOPT-central_difference_interval:


Central Difference Interval
===========================



:Type:	Floating point number	
:Range:	[0,1] + {na}	
:Default:	na	



When the value of **Derivative Option**  equals 'Some gradients are unknown', 
the value of this option, denoted by r, is used near an optimal solution 
to obtain more accurate (but more expensive) estimates of gradients. 
Twice as many function evaluations are required compared to forward differencing. 
The interval used for the jth variable is :math:`hr = r(1+| xj |)`. 
The resulting gradient estimates should be accurate to O(r2), unless the functions are badly scaled.



The default value of this option depends on the relative precision of the computer being used. 
On most computers the default equals 6.0e-6.



**Learn more about** 

*	:ref:`option-SNOPT-derivative_option`  
