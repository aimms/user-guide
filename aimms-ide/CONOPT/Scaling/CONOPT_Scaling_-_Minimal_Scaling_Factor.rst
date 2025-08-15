.. _CONOPT_Scaling_-_Minimal_Scaling_Factor:

Minimal Scaling Factor
======================



:Type:	Floating point number	
:Range:	[1e-10,1.0]	
:Default:	1.0	



Scale factors used to scale variables and equations are projected on the range **Minimal Scaling Factor**  to **Maximal Scaling Factor** . The limits are used to prevent very large or very small scale factors due to pathological types of constraints. The default value for this option is 1 which means that small values are not scaled up. If you need to scale small value up towards 1 then you must define a value < 1.



**Learn more about** 

*	:ref:`CONOPT_Scaling_-_Maximal_Scaling_Factor`  
