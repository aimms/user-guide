

.. _IPOPT_NLP_-_Assume_quadratic_problem:


Assume quadratic problem
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option indicates whether the problem is a quadratic problem. Activating this option will cause IPOPT to ask for the Hessian of the Lagrangian function only once for the NLP and reuse this information later. Possible values are:



*	No
*	Yes



