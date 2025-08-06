.. _SNOPT_Advanced_-_Pivot_Tolerance:


Pivot Tolerance
===============



**Type** :	Floating point number	

**Range** :	[0,1] + {na}	

**Default** :	na	



During the solve of QP subproblems, the pivot tolerance is used to prevent columns entering the basis if they would cause the basis to become almost singular.



When x changes to x+ap for some search direction p, a "ratio test" is used to determine which component of x reaches an upper or lower bound first. The corresponding element of p is called the pivot element. Elements of p are ignored (and therefore cannot be pivot elements) if they are smaller than the pivot tolerance.



It is common for two or more variables to reach a bound at essentially the same time. In such cases, the **Feasibility Tolerance**  provides some freedom to maximize the pivot element and thereby improve numerical stability. Excessively small values for the **Feasibility Tolerance**  should therefore not be specified. To a lesser extent, the **Expand Frequency**  also provides some freedom to maximize the pivot element. Excessively large values for the **Expand Frequency**  should therefore not be specified.



The default value of this option depends on the relative precision of the computer being used. On most computers the default equals 3.7e-11.



**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Expand_Frequency`  
*	:ref:`SNOPT_Feasibility_-_Feasibility_Tole`  



