.. _option-CBC-integrality:


Integrality
===========



:Type:	Floating point number	
:Range:	[1e-20,0.5]	
:Default:	1e-6	



This option specifies the integer feasibility tolerance (MIP only). For an optimal solution no integer variable may be this away from an integer value. 



If this option is set too small, CBC may falsely conclude that the problem is infeasible.



**Note** 

*	Beware of setting this smaller than the **Primal Feasibility Tolerance**.




**Learn more about** 

*	:doc:`CBC_General_-_Primal_feasibility_tol <../General/CBC_General_-_Primal_feasibility_tol>`  
