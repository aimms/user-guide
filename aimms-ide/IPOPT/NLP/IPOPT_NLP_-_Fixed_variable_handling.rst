

.. _IPOPT_NLP_-_Fixed_variable_handling:


Fixed variable handling
=======================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Convert to parameter	



This option determines how fixed variables should be handled. Possible values are:



*	Convert to parameter
*	Add equality constraints
*	Relax fixing bound constraints




The main difference between the possible settings is that the starting point in the 'Add equality constraints' case still has the fixed variables at their given values, whereas in the case 'Convert to parameter' the functions are always evaluated with the fixed values for those variables. Also, for Relax fixing bound constraints', the fixing bound constraints are relaxed (according to the value of option**Factor for Initial Bounds Relaxation** ). For both 'Add equality constraints' and 'Relax fixing bound constraints', bound multipliers are computed for the fixed variables.





**Learn more about** 

*	:ref:`IPOPT_NLP_-_Factor_for_initial_bounds_relaxation` 
