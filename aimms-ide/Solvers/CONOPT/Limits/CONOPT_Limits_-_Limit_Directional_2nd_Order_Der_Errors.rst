.. _option-CONOPT-limit_on_directional_2nd_order_derivative_errors:

Limit on Directional 2nd Order Derivative Errors
================================================



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	10	



If the evaluation of Directional Second Derivatives (Hessian information in a particular direction) has failed more than **Limit on 2nd Order Derivative Errors**  times, CONOPT will not attempt to evaluate them any more and will switch to methods that do not use Directional Second Derivatives. Note that second order information may not be defined even if function and derivative values are well-defined, e.g. in an expression like power(x,1.5) at x=0.

