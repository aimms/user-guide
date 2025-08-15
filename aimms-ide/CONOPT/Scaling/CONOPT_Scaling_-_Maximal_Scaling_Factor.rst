.. _CONOPT_Scaling_-_Maximal_Scaling_Factor:

Maximal Scaling Factor
======================



:Type:	Floating point number	
:Range:	[128,1e+10]	
:Default:	1024	



Scale factors are projected on the interval from **Minimal Scaling Factor**  to **Maximal Scaling Factor** . The limits are used to prevent very large or very small scale factors due to pathological types of constraints. The upper limit is selected such that Square(X) can be handled for X close to **Maximum Solution of a Variable** . More nonlinear functions may not be scalable for very large variables.



**Learn more about** 

*	:ref:`CONOPT_Limits_-_Maximal_Solution_Variable`  
*	:ref:`CONOPT_Scaling_-_Minimal_Scaling_Factor`  
