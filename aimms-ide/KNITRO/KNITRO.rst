

KNITRO
======

**Description** 

Artelys Knitro is a software package for solving nonlinear programming problems with or without complementarity constraints. The general nonlinear programming problem with complementarity constraints (MPCC) can be expressed in the following form:






.. list-table::

   * - ``minimize`` (x,y)
     - f(x,y)
     - 
   * - ``subject to`` 
     - Lj ≤ gj(x,y) ≤ Uj
     -  j Î J
   * - 
     - li ≤ xi ≤ ui 
     -  i Î I
   * - 
     - Lk ≤ hk(x,y) ≤ Uk ^ lk ≤ yk ≤ uk 
     -  k Î C




where I Ç C = Æ and J Ç C = Æ, and

(x,y) is the vector of variables,

l and u are vectors of lower and upper bounds on the variables,

f is a differentiable (nonlinear) function,

(g,h) is a vector of differentiable nonlinear functions, and

L and U are vectors of lower and upper bounds on g and h.



Some of the lower bounds may be – ¥ and some of the upper bounds may be + ¥. The last group of conditions represent the complementarity conditions. The vector x denotes the normal variables while y represents the complementarity variables. For the complementarity conditions it holds that exactly two of the bounds on the variables and constraints should be finite. See the next section for how complementarity conditions are defined in AIMMS.



If there are no complementarity conditions (i.e., C = Æ), then the resulting problem in a nonlinear programming problem (NLP). Knitro 14.0 can also be used for solving nonlinear programming problems in which some or all of the variables must assume integer values in the solution. Such problems are known as mixed integer nonlinear programs or MINLPs. Knitro cannot handle problems that contain complementarity constraints as well as integer variables.



Knitro is designed for finding local solutions but multistart heuristics are provided for trying to locate the global solution. Knitro is designed for solving large-scale continuous, smooth optimization problems. Problems with derivative discontinuities can also often be solved successfully. Knitro implements both state-of-the-art interior-point and active-set methods for solving nonlinear optimization problems.



Knitro is equipped with parameters that influence the performance of Knitro. AIMMS is equipped with options that set the parameters in Knitro. Options in AIMMS can be set in the options dialog box.



Note that the general solvers option **Iteration Limit**  defines (in case of Knitro) a limit on the number of major iterations. The general solvers option **Time Limit**  defines the maximum allowable CPU time before termination.



Knitro can use its own multistart algorithm. It the option **Multistart**  is switched on then Knitro will solve from multiple start points and try to find a better solution.



Knitro 14.0 supports the :ref:`KNITRO_Tuner` , a utility to aid you in improving the performance of your optimization application. It suggests a suite of option settings for you to use that provide better performance than the default option settings for your model.



The option categories MIP and MIP Cuts contain options that influence the Knitro algorithm for solving MINLP problems.





**Presolving** 

AIMMS contains a presolve algorithm with the goal to reduce the size of the problem and to tighten the variable bounds, 
which may help Knitro to solve nonlinear problems faster. 
Knitro is a local solver, i.e., the solution found by the Knitro is a local solution and cannot be guaranteed to be a global solution. 
The presolve algorithm may help the solver in finding a better solution. 
A local solver might sometimes fail to find a solution and then it is not always clear whether that is caused 
by the problem being infeasible or by the solver failing to find a solution for a feasible problem. 
The presolve algorithm may reveal inconsistent constraints and/or variable bounds and hence identify a problem as infeasible.



The AIMMS presolver is switched off by default. To use it you should switch on the AIMMS general solvers option **Nonlinear Presolve** .



Please note that, by default, Knitro uses its own presolver which is less powerful than the AIMMS presolver. 
The Knitro presolver is controlled by the option **Presolve** .



**Parallel solves** 

Knitro 14.0 is thread-safe and therefore multiple nonlinear mathematical program instances can be solved in parallel using Knitro 14.0 (assuming your computer has multiple processors or a multi-core processor). 
The function GMP::SolverSession::AsynchronousExecute should be used to solve multiple mathematical program instances in parallel.



**Learn more about** 

*	`Knitro <https://web.stanford.edu/group/SOL/home_software.html>`_ (Internet link)
*	:ref:`KNITRO_KNITRO140_to_AIMMS_Mapping` 
*	:ref:`KNITRO_AIMMS_to_KNITRO140_Mapping`  
*	:ref:`KNITRO_Description_KNITRO140_Algorithms` 
*	:ref:`KNITRO_Complementarities` 
*	:ref:`KNITRO_Tuner` 
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`Options_Stop_Criteria_-_Iteration_Limi`  
*	:ref:`KNITRO_MS_-_Multistart`  
*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 
*	:ref:`KNITRO_Presolve_-_Presolve`  
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
