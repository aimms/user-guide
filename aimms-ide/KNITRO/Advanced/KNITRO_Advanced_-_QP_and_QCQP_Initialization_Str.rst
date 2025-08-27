.. _option-KNITRO-qp_and_qcqp_initialization_strategy:


QP and QCQP Initialization Strategy
===================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies the initialization strategy used for non-convex QPs and QCQPs. In particular, these strategies may be more likely to cause Knitro to find global or better local solutions on non-convex quadratic programs (QPs) or non-convex quadratically constrained quadratic programs (QCQPs). Possible values are:



    *	Automatic
    *	None
    *	Linear
    *	Hybrid
    *	Penalty
    *	Convex Quadratic




By setting 'Automatic' Knitro will automatically determine the strategy. 'None' indicates that no special initialization strategy will be used. Setting 'Linear', 'Hybrid', 'Penalty', and 'Convex Quadratic' results in initializing by solving a linear relaxation, a hybrid formulation, a penalty formulation, and a convex quadratic relaxation, respectively.




