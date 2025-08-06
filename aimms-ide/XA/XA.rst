 

XA
==

**Description** 

XA (version 16) is a tool for solving, first of all, linear optimization problems. Such problems are conventionally written like this:



``Minimize (or Maximize) c1x1 + cx2 + .. + cnxn;`` 

``Subject to:`` 

``a11x1 + a12x2 + … + a1nxn ~ b1`` 

``a11x1 + a12x2 + … + a1nxn ~ b1`` 

``…`` 

``a11x1 + a12x2 + … + a1nxn ~ b1`` 

``l1<= x1 <=u1, …, ln <= xn <= un`` 



where,

x is the vector of variables,

a,b, and c real numbers.

l and u are vectors of lower and upper bounds, and

~ can be either <=, >=, or =.



Some of the lower bounds may be –inf and some of the upper bounds may be inf. The scalar value n will denote the number of variables and m the number of equations. XA can also solve binary, integer and semi continuous linear programming problems.



XA is equipped with parameters that influence the performance of XA. AIMMS is equipped with options that set the parameters in XA. Options in AIMMS can be set in the options dialog box.



XA 16 offers three methods for solving LP problems, the primal simplex method, the dual simplex method and the barrier method (also called interior-point method). The barrier method is the fastest for most LP problems, but when the barrier method is used no sensitivity information (e.g. shadow prices and reduced costs) is available.



XA 16 can also handle certain problems in which the objective function is not linear but quadratic. (The constraints in such a problem are still linear). Such problems are known as quadratic programs or QPs. 



**Learn more about** 

*	XA official site: ``http://www.sunsetsoft.com`` (Internet link)
*	:ref:`XA_to_AIMMS_Mapping`  
*	:ref:`XA_AIMMS_to_XA_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`Miscellaneous_Solver_Configuration` 
*	:ref:`XA_Troubleshooting`  



