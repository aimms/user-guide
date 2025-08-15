.. _ODH-CPLEX_XGeneral_-_MemoryEmphasis:


Memory Emphasis
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option lets you indicate to CPLEX that it should conserve memory where possible. When you set this option to its nondefault value, CPLEX will choose tactics, such as data compression or disk storage, for some of the data computed by the barrier and MIP optimizers. Of course, conserving memory may impact performance in some models. Also, while solution information will be available after optimization, certain computations that require a basis that has been factored (for example, for the computation of the condition number 'kappa') may be unavailable.



Possible values of this option are:



*	No
*	Yes



