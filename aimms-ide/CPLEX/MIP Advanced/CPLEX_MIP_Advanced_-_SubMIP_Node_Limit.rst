.. _option-CPLEX-submip_node_limit:


SubMIP Node Limit
=================



:Type:	Integer	
:Range:	{1 .. 2100000000}	
:Default:	500	



The option sets the number of nodes explored when CPLEX is solving a subMIP of a MIP. SubMIPS are described in the section :ref:`option-CPLEX-submip` .



**Note** 

*	This rarely used option is helpful **only**  in rare "corner" cases where there is clear evidence that the default limit is really inappropriate for this particular problem.




**Learn more about** 

*	:ref:`option-CPLEX-submip` 
