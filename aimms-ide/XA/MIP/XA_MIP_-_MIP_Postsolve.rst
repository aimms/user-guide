.. _XA_MIP_-_MIP_Postsolve:


MIP Postsolve
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Round before solving final LP	



XA does not round the found integer values of a MIP to the nearest integer value. Instead it returns values which are considered to be integer within tolerances. This option offers the possibility to perform some post-solving on the found solution concerning rounding of values for the integer variables and computing marginal values and a basis. The following methods are available:



*	No rounding (the found values for the integer variables are not rounded to the nearest integer value and that no basis and marginals are computed)
*	Round to integer (the found values for the integer variables are rounded to the nearest integer value, but no basis and marginal values are computed)
*	Solve final LP (no rounding) (the final LP is solved again to obtain the marginal values and a basis. The found values for the integer variables are not rounded)
*	Solve final LP (round) (the final LP is solved again to obtain the marginal values and a basis. Afterwards the found values for the integer variables are rounded to the nearest integer value)
*	Round before solving final LP (prior to solving the final LP, the found values for the integer variables are rounded to the nearest integer value. This implies that the LP is solved with all integer variables fixed, which results in the true integer solution of the MIP. In addition marginal values and a basis are available as well. In a few special cases a feasible model can become infeasible as a result of fixing the integer variables. In such a case post-solving of type "round to integer" or "solve final LP (round)" will be performed, depending on whether post-solving of the latter type returns a feasible solution. Furthermore, a message will be displayed to notify the user of the performed relaxation of this option)




**Learn more about** 

*	:ref:`XA_MIP_-_Lower_Integer_Tolerance`  
*	:ref:`XA_MIP_-_Upper_Integer_Tolerance`  



