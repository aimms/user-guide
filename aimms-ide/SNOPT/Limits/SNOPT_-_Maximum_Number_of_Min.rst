.. _SNOPT_-_Maximum_Number_of_Min:


Maximum Number of Minor Iterations
==================================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	500	



If the number of minor iterations for the optimality phase of the QP subproblem exceeds the limit set by this option, then all nonbasic QP variables that have not yet moved are frozen at their current values and the reduced QP is solved to optimality. More minor iterations may be necessary to solve the reduced QP to optimality. These extra iterations are necessary to ensure that the terminated point gives a suitable direction for the line search.



Note that the global solvers option **Iteration Limit**  defines (in case of SNOPT) an independent limit on the number of major iterations. (A major iteration consists of solving a QP subproblem.)



**Learn more about** 

*	:ref:`SNOPT_Limits_-_Maximum_Number_of_Tot`  



