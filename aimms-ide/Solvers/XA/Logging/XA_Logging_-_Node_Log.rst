.. _option-XA-node_log:


Node Log
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines if and how listings of the nodes examined during the branch and bound process of the MIP solver are produced. In case of the value full, iteration messages for each node are printed. Possible values are:



    *	No
    *	Yes
    *	Full




The output produced by this option can only be noticed if either the option **Solver Window Message**  or the option **Solver Listing Messages**  is set to one of the values "Remark" or "All". In case of the latter option, the option **Solver Listing** should be set to a value different from "Never" as well.





**Learn more about** 

*	:ref:`option-AIMMS-solver_window_messages`  
*	:ref:`option-AIMMS-solver_listing`  
*	:ref:`option-AIMMS-solver_listing_messages`  



