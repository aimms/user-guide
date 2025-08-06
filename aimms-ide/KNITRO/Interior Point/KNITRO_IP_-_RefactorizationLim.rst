.. _KNITRO_IP_-_RefactorizationLim:


Refactorization Limit
=====================



**Type** :	Integer	

**Range** :	{-1..1000000}	

**Default** :	-1	



This option indicates the maximum number of refactorizations of the KKT system per iteration of the Interior/Direct algorithm before reverting to a CG step. These refactorizations are performed if negative curvature is detected in the model. Rather than reverting to a CG step, the Hessian matrix is modified in an attempt to make the subproblem convex and then the KKT system is refactorized. Increasing this value will make the Interior/Direct algorithm less likely to take CG steps. If the Interior/Direct algorithm is taking a large number of CG steps (as indicated by a positive value for "CG its" in the output), this may improve performance.



If this value is set to -1 then Knitro will use a dynamic strategy.



This option has no effect on the Active Set and SQP algorithms.



**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 



