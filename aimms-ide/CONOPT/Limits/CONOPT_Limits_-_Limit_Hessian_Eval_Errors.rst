.. _CONOPT_Limits_-_Limit_Hessian_Eval_Errors:

Limit on Hessian Evaluation Errors
==================================



**Type**:	Integer	

**Range**:	{0..:ref:`Miscellaneous_Maxint` }	

**Default**:	10	



If the evaluation of Hessian information has failed more than **Limit on Hessian Evaluation Errors**  times, CONOPT will not attempt to evaluate it any more and will switch to methods that do not use the Hessian. Note that second order information may not be defined even if function and derivative values are well-defined, e.g. in an expression like power(x,1.5) at x=0.

