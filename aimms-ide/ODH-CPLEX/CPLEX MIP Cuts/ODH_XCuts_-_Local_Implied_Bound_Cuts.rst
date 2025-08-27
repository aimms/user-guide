.. _option-ODHCPLEX-local_implied_bound_cuts:


Local Implied Bound Cuts
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether or not to generate locally valid implied bound cuts for the problem. Setting the value to "Automatic", the default, indicates that the attempt to generate implied bound cuts should continue only if it seems to be helping. Possible values are:



    *	Off
    *	Automatic
    *	Generate cuts moderately
    *	Generate cuts aggressively
    *	Generate cuts very aggressively




In some models, binary variables imply bounds on nonbinary variables (that is, general integer variables and continuous variables). CPLEX generates cuts to reflect these relationships. In fact, CPLEX can generate two different types of implied bound cuts:





*   CPLEX generates global implied bound cuts by using globally valid bounds on the continuous variables in the model. The option **Implied Bound Cuts**  controls this activity.
*   CPLEX generates local implied bound cuts by using locally valid bounds on the continuous variables of the subproblem (that is, the branch-and-bound node) under consideration. This option controls this activity.




**Learn more about** 

*	:ref:`option-ODHCPLEX-implied_bound_cuts`  
