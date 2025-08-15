.. _GUROBI_Quadratic_-_QCP_Dual_Values:


QCP Dual Values
===============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option determines whether dual variable values are computed for QCP models. Computing them can add significant time to the optimization, so you should only set this option to 'Yes' if you need them. Possible values are:



*	No
*	Yes




**Note** 

*	Dual variables values are not computed if the option **Nonconvex Strategy**  is set to 'Translate'.




**Learn more about** 

*	:ref:`GUROBI_Quadratic_-_Nonconvex_Strategy` 
