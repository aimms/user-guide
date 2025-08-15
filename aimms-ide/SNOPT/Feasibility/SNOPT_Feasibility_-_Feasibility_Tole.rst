.. _SNOPT_Feasibility_-_Feasibility_Tole:


Feasibility Tolerance
=====================



:Type:	Floating point number	
:Range:	[0,1000]	
:Default:	1e-6	



SNOPT tries to ensure that all variables eventually satisfy their upper and lower bounds to within the tolerance defined by the value of this option. This includes slack variables. Hence, the general constraints are also satisfied to within the feasibility tolerance.



If the bounds and linear constraints cannot be satisfied to within the feasibility tolerance, the problem is declared infeasible. If the sum of infeasibilities is quite small, it may be appropriate to raise the feasibility tolerance by a factor 10 or 100. Otherwise, some error in the data should be suspected.



Nonlinear functions will be evaluated only at points that satisfy the bounds and linear constraints. If there are regions where a function is undefined, every attempt should be made to eleminate these regions from the problem. For example, if f(x) = Öx1 + log(x2), it is essential to place lower bounds on both variables x1 and x2. If the feasibility tolerance equals 1e-6, the bounds x1 >= 1e-5 and x2 >= 1e-4 might be appropriate. (The log singularity is more serious. In general, keep x as far away from singularities as possible.)



If scaling is used (i.e., the value of the option **Scale Method**  is not equal to 'No scaling'), feasibility is defined in terms of the scaled problem (since it is then more likely to be meaningful).



In reality, SNOPT uses the feasibility tolerance for satisfying the bounds on x and s in each QP subproblem. If the sum of infeasibilities cannot be reduced to zero, the QP subproblem is declared infeasible. SNOPT is the in "elastic mode" thereafter (with only the linearized nonlinear constraints defined to be elastic). See the option **Elastic Weight** .



**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Elastic_Weight`  
*	:ref:`SNOPT_Scaling_-_Scale_Method`  



