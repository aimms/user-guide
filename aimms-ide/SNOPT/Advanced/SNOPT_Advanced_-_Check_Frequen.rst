.. _option-SNOPT-check_frequency:


Check Frequency
===============



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	60	



Let k denote the value of this option. Every kth (minor) iteration after the most recent basis factorization, a numerical test is made to see if the current solution x satisfies the general linear constraints (including linearized nonlinear constraints, if any). The constraints are of the form Ax – s = b, where s is the set of slack variables. To perform the numerical test, the residual vector r = b – Ax + s is computed. If the largest component of r is judged to be too large, the current basis is refactorized and the basic variables are recomputed to satisfy the general constraints more accurately. 



