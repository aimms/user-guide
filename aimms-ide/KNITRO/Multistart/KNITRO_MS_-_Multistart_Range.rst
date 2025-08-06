.. _KNITRO_MS_-_Multistart_Range:


Multistart Range
================



**Type** :	Floating point number	

**Range** :	[0,1e20]	

**Default** :	1000



This option specifies the maximum range that each variable can take when determining new start points. If a variable has upper and lower bounds and the difference between them is less than the value of this option, then new start point values for the variable can be any number between its upper and lower bounds. If the variable is unbounded in one or both directions, or the difference between bounds is greater than the minimum of the value of this option and the value of option **Multistart Range Unbounded Variable** , then new start point values are restricted by this option. If x is such a variable, then all initial values satisfy



	max{ bL, x0 - t  } ≤ x ≤ min{ bU, x0 + t },

	t = min{ r/2, η/2} 



where x0 is the initial value of x provided by the user, bL and bU are the variable bounds (possibly infinite) on x, r is the value of this option and η the value of option **Multistart Range Unbounded Variable** .



This option has only effect if the option **Multistart**  is switched on.



**Learn more about** 

*	:ref:`KNITRO_MS_-_Multistart`  
*	:ref:`KNITRO_MS_-_Multistart_Range_Unbounded_Var`  
