.. _CONOPT_Scaling_-_Scaling_Method:

Scaling Method
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Largest term	



This option specifies the method used by CONOPT for scaling. Possible values are:



*	Geometric mean
*	Largest term variant
*	Moving average
*	Largest term




CONOPT will by default use scaling of the equations and variables of the model to improve the numerical behavior of the solution algorithm and the accuracy of the final solution (see also the option **Rescaling Frequency** ). The objective of the scaling process is to reduce the values of all large primal and dual variables as well as the values of all large first derivatives so they become closer to 1. Small values are usually not scaled up, see the options **Minimal Scaling Factor**  and **Maximal Scaling Factor** . The default scaling method is recommended. The others are only kept for backward compatibility.





Default value 'Largest term': Rows are first scaled by dividing by the largest term in the row, then columns are scaled by dividing by the maximum of the largest term and the value of the variable. A term is here defined as abs(X)*abs(Jac) where X is the value of the variable and Jac is the value of the derivative (Jacobian element). The scale factor are then projected on the interval between **Minimal Scaling Factor**  and **Maximal Scaling Factor** .





Value 'Geometric mean': Scaling is based on repeatedly dividing the rows and columns by the geometric means of the largest and smallest elements in each row and column. Very small elements less than the value specified by the option **Minimal Jacobian Element for Scaling**  are considered equal to the value of that option.





Value 'Largest term variant': Similar to 'Largest term' above, but the projection on the interval [**Minimal Scaling Factor** ,**Maximal Scaling Factor** ] is applied at a different stage. With method 'Geometric mean', abs(X)*abs(Jac) with small X and very large Jac is scaled very aggressively with a factor abs(Jac). With method 'Largest term', the scale factor is abs(X)*abs(Jac). The difference is seen in models with terms like Sqrt(X) close to X = 0.





Value 'Moving average': As 'Geometric mean' but the terms are computed based on a moving average of the squares X and Jac. The purpose of the moving average is to keep the scale factor more stable. This is often an advantage, but for models with very large terms (large variables and in particular large derivatives) in the initial point the averaging process may not have enough time to bring the scale factors into the right region.





**Learn more about** 

*	:ref:`CONOPT_Scaling_-_Maximal_Scaling_Factor`  
*	:ref:`CONOPT_Scaling_-_Minimal_Jacobian_Element_Scaling`  
*	:ref:`CONOPT_Scaling_-_Minimal_Scaling_Factor`  
*	:ref:`CONOPT_Scaling_-_Rescale_frequency`  
