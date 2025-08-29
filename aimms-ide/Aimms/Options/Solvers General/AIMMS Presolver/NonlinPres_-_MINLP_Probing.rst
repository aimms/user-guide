

.. _option-AIMMS-minlp_probing:


MINLP Probing
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Limited	


This option controls whether the AIMMS Presolver should do probing for MINLP models (and for MIP, MIQP and MIQCP models).
Probing is a technique that looks at the logical implications of fixing a binary variable to 0 or 1. Possible values are:


    *	Off
    *	Limited
    *	More
    *	Full


With setting 'Limited' only very basic probing is done. The AIMMS Presolver will try to transform some classes of
nonlinear constraints if the option **Reformulate Constraints** is switched on.

If setting 'More' is selected then probing will also apply coefficient improvement using bound reduction. Coefficient
improvement is a process of improving the coefficients of the binary variables such that the NLP relaxation becomes
more tight. More about coefficient improvement can be found in the paper by Johnson et al. (2000).

If setting 'Full' is selected then probing will try coefficient improvement more aggressively. Full probing can
result in more (binary) variables being removed. This setting can be computationally expensive.


**Note** 

*	This option has only an effect when solving a nonlinear model and the option **Nonlinear Presolve** is switched on, or when solving a linear, quadratic or quadratically-constrained model and the option **Linear Presolve** is switched on, or if the function :any:`GMP::Instance::CreatePresolved` is used.
*	If the function :any:`GMP::Instance::CreatePresolved` is used then AIMMS will change the model type from MINLP (NLP) into MIP (LP) if this option is switched on and the presolved model contains no nonlinear constraints.
*	Probing can significantly improve the performance of the solvers CBC and XA for MIP models.


**Learn more about** 

*	:ref:`option-AIMMS-linear_presolve` 
*	:ref:`option-AIMMS-nonlinear_presolve`  
*	:ref:`option-AIMMS-reformulate_constraints`  


**References** 

*	Johnson, E.L., G.L. Nemhauser and M.W.P. Savelsbergh, Progress in Linear Programming-Based Algorithms for Integer Programming: An Exposition, INFORMS Journal on Computing **12(1)**  (2000), pp. 2-23.
*	Savelsbergh, M.W.P., Preprocessing and probing techniques for mixed integer programming problems, ORSA Journal on Computing **6**  (1994), pp. 445-454.
