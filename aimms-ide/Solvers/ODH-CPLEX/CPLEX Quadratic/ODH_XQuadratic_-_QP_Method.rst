.. _option-ODHCPLEX-qp_method:


QP Method
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines which algorithm is used for solving QP problems and MIQP subproblems. Possible values are:



    *	Automatic
    *	Primal simplex
    *	Dual simplex
    *	Network simplex
    *	Barrier




**Note** 

*	The barrier algorithm can use parallel processes (threads) as controlled by the option **Global Thread Limit**.




**Learn more about** 

*	:doc:`ODH_XPar_-_GlobalThreadLimit <../CPLEX Parallel/ODH_XPar_-_GlobalThreadLimit>`  



