.. _option-XA-mip_strategy:


MIP Strategy
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Proprietary method	



This option can be used to select one of the nine branch and bound strategies supported by XA. Each XA branch and bound strategy has three variations that can be set by means of the options **MIP Strategy Branching Priorities**, **MIP Strategy Estimate Integer Solution**  and **MIP Strategy Split Node List**. In some cases these variations reduce the solution time but may not yield an optimal integer solution. If you are interested in obtaining a fast and 'good' integer solution (which may not be optimal) try these variations. Possible values of this option are:



    *	Proprietary method
    *	Minimum change in objective function
    *	Priority based on column order
    *	Column closest to its integer bound
    *	(Not used)
    *	Column always branches up
    *	Column always branches down
    *	Column farthest from its integer bound
    *	Column randomly selected
    *	Apparent smoothest sides in the polytope




The setting "Column randomly selected" is useful when solving very large problems.





**Learn more about** 

*	:ref:`option-XA-mip_strategy_branching_priorities`  
*	:ref:`option-XA-mip_strategy_estimate_integer_solution`  
*	:ref:`option-XA-mip_strategy_split_node_list`  



