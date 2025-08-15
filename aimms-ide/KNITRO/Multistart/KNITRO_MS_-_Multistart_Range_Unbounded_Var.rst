.. _KNITRO_MS_-_Multistart_Range_Unbounded_Var:


Multistart Range Unbounded Variable
===================================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	1e20



This option specifies the maximum range that an unbounded variable can take when determining new start points. If a variable is unbounded in one or both directions, then new start point values are restricted by the option. If x is such a variable, then all initial values satisfy



	max{ bL, x0 - η/2  } ≤ x ≤ min{ bU, x0 + η/2 },



where x0 is the initial value of x provided by the user, bL and bU are the variable bounds (possibly infinite) on x and η is the value of this option.



This option has only effect if the option **Multistart**  is switched on.



**Learn more about** 

*	:ref:`KNITRO_MS_-_Multistart`  
*	:ref:`KNITRO_MS_-_Multistart_Range`  
