.. _KNITRO_Hessian_-_SecondOrderCor:


Second Order Correction
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	At some iterations	



This option indicates whether or not the second order correction (SOC) option should be used. A second order correction may be beneficial for problems with highly nonlinear constraints. Possible values are:



*	None
*	At some iterations
*	Always




With setting 'At some iterations' second order correction steps may be attempted on some iterations. With setting 'Always' second order correction steps are always attempted if the original step is rejected and there are nonlinear constraints.




