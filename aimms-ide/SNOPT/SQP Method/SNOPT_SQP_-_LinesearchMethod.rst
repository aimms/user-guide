.. _SNOPT_SQP_-_LinesearchMethod:


Linesearch Method
=================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Derivative linesearch	



At each major iteration a line search is used to improve the merit function. A 'Derivative linesearch' uses safeguarded cubic interpolation and requires both function and gradient values to compute estimates of the step ak. If some analytic derivatives are not provided, or a 'Nonderivative linesearch' is specified, SNOPT employs a line search based upon safeguarded quadratic interpolation, which does not require gradient evaluations.



A nonderivative line search can be slightly less robust on difficult problems, and it is recommended that the default be used if the functions and derivatives can be computed at approximately the same cost. If the gradients are very expensive relative to the functions, a nonderivative line search may give a significant decrease in computation time.



Possible values are:



*	Derivative linesearch
*	Nonderivative linesearch




**Learn more about** 

*	:ref:`SNOPT_SQP_-_DerivativeOption`  
