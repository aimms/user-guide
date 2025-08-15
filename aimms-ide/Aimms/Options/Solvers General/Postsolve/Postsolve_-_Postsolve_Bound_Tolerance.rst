

.. _Options_Postsolve_-_Postsolve_Bound_Tolerance:


Postsolve Bound Tolerance
=========================



**Type**:	Floating point number	

**Range**:	[0,0.1]	

**Default**:	1e-10	



This option specifies the bound tolerance used for continuous variables. If the postsolve is active then AIMMS will check whether all continuous variables have solution values that are inside the variable bounds, allowing for small violations as specified by this option. If at least one of the continuous variables has a solution value that violates one of its bounds, and the violation is larger than the value of this option, then the option **Postsolve Continuous Variables**  specifies how the postsolve step will handle those violated variables.



**Note** 

*	This option was introduced in AIMMS 4.85. AIMMS 4.84 and older used a fixed bound tolerance of 0. To get the old behavior you should set this option to 0.




**Learn more about** 

*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`Options_Postsolve_-_Postsolve_Continuous_Variables` 



