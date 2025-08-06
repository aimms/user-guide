

CBC
===

**Description** 

CBC is a tool for solving linear optimization problems. Such problems are conventionally written like this:



``Minimize (or Maximize)`` c1x1 + c2x2 + ... + cnxn

``Subject to:`` 

a11x1 + a12x2 + … + a1nxn ~ b1

a21x1 + a22x2 + … + a2nxn ~ b2

  …

am1x1 + am2x2 + … + amnxn ~ bm

l1 <= x1 <= u1, …, ln <= xn <= un



where,

x is the vector of variables,

a, b, and c are real numbers,

l and u are vectors of lower and upper bounds, and

~ can be either <=, >=, or =.



Some of the lower bounds may be –inf and some of the upper bounds may be inf. The scalar value n will denote the number of variables and m the number of equations.



In the most basic linear optimization problem, the variables of the objective function are continuous in the mathematical sense, with no gaps between real values. CBC can also be used for solving linear programming problems in which some or all of the variables must assume integer values in the solution. Such problems are known as mixed integer programs or MIPs. 



CBC is equipped with parameters that influence the performance of CBC. AIMMS is equipped with options that set the parameters in CBC. Options in AIMMS can be set in the options dialog box.



In CBC it is possible to use a solution as a MIP start by setting the option **MIP Start** .



**COIN-OR** 

CBC is an open-source solver and available from COIN-OR. The Computational Infrastructure for Operations Research (COIN-OR) project is an initiative to spur the development of open-source software for the operations research community.



The source code of CBC is available at COIN-OR. The code has been written by primarily by John J. Forrest. The source code of the AIMMS-CBC link is available from the AIMMSlinks project at COIN-OR. See the Internet links below.



**Deprecated postsolve options** 

The postsolve step for linear models has been moved from the solver interface of CBC to AIMMS. The postsolve options of CBC have been replaced by general solvers options with similar names. See the new general solvers option **Postsolve**  for more information.



**Learn more about** 

*	`CBC <https://github.com/coin-or/Cbc>`_ (Internet link)
*	`COIN-OR <https://www.coin-or.org/>`_ (Internet link)
*	`AIMMSlinks <https://github.com/coin-or/AIMMSlinks>`_ (Internet link)
*	:ref:`CBC_CBC_2_4_to_AIMMS_Mapping`  
*	:ref:`CBC_AIMMS_to_CBC_2_4_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`CBC_MIP_-_MIP_Start` 
*	:ref:`Options_Postsolve_-_Postsolve` 
