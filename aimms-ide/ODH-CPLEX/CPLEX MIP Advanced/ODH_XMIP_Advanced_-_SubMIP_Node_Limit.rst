.. _ODH-CPLEX_XMIP_Advanced_-_SubMIP_Node_Limit:


SubMIP Node Limit
=================



**Type** :	Integer	

**Range** :	{1 .. 2100000000}	

**Default** :	500	



The option sets the number of nodes explored when CPLEX is solving a subMIP of a MIP. SubMIPS are described in the section 'SubMIP' of the CPLEX 20.1 help.



**Note** 

*	This rarely used option is helpful **only**  in rare "corner" cases where there is clear evidence that the default limit is really inappropriate for this particular problem.



