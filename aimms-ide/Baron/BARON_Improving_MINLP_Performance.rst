

.. _Baron_Improving_MINLP_Performance:


Improving MINLP Performance
===========================

**Presolving** 

One way of improving the performance of BARON when solving a MINLP problem is by switching on the AIMMS nonlinear presolve algorithm as controlled by the general solvers option **Nonlinear Presolve** . The nonlinear presolver can reduce the size of the problem and tighten the variable bounds which might help BARON to solve nonlinear problems faster. It might help to increase the amount of probing done by the nonlinear presolver; this is controlled by the general solvers option **MINLP Probing** .



**Using solution found by another MINLP solver** 

For some MINLP problems the performance of BARON can get a boost by providing a good feasible integer solution. Such feasible integer solution can be found by first solving the MINLP problem using the MINLP solver AOA before calling BARON. In that case BARON will automatically use the integer solution found by AOA as an incumbent solution. AOA is usually much faster than BARON but AOA cannot guarantee to find a global optimum solution (unless the model is convex).



**Learn more about** 

*	:ref:`Options_NonlinPres_-_MINLP_Probing` 
*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 



