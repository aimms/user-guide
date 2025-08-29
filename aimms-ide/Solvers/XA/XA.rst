.. _SolverXA: 

XA
==

**Description** 

XA (version 16) is a tool for solving, first of all, linear optimization problems. Such problems are conventionally written like this:

.. math::

   \begin{aligned}
   & \text{Minimize:} \quad && c_{1}x_{1} + c_{2}x_{2} + \ldots + c_{n}x_{n} \\
   & \text{Subject to:} \\
   & && a_{11}x_{1} + a_{12}x_{2} + \ldots + a_{1n}x_{n} \sim b_1 \\
   & && a_{21}x_{1} + a_{22}x_{2} + \ldots + a_{2n}x_{n} \sim b_2 \\
   & && \vdots \\
   & && a_{m1}x_{1} + a_{m2}x_{2} + \ldots + a_{mn}x_{n} \sim b_m \\
   & && l_1 \leq x_1 \leq u_1 \\
   & && \vdots \\
   & && l_n \leq x_n \leq u_n
   \end{aligned}

where,

* :math:`x` is the vector of variables,
* :math:`a`, :math:`b`, and :math:`c` are real numbers,
* :math:`l` and :math:`u` are vectors of lower and upper bounds, and
* :math:`\sim` can be either <=, >=, or =.

Some of the lower bounds may be :math:`-\infty` and some of the upper bounds may be :math:`\infty`.
The scalar value :math:`n` denotes the number of variables and :math:`m` the number of equations. XA can also solve binary, integer and semi continuous linear programming problems.

The optimization problem can be maximized instead of minimized.

XA is equipped with parameters that influence the performance of XA. AIMMS is equipped with options that set the parameters in XA. Options in AIMMS can be set in the options dialog box.



XA 16 offers three methods for solving LP problems, the primal simplex method, the dual simplex method and the barrier method (also called interior-point method). The barrier method is the fastest for most LP problems, but when the barrier method is used no sensitivity information (e.g. shadow prices and reduced costs) is available.



XA 16 can also handle certain problems in which the objective function is not linear but quadratic. (The constraints in such a problem are still linear). Such problems are known as quadratic programs or QPs. 



**Learn more about** 

*	`XA <http://www.sunsetsoft.com>`_ (Internet link)
*	:ref:`XA_to_AIMMS_Mappings`  
*	:ref:`AIMMS_to_XA_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`Miscellaneous_Solver_Configuration` 
*	:ref:`XA_Troubleshooting`  



