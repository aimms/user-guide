.. _CPLEX_Prepr_-_Pre_reduction_types:


Preprocessing Reduction Types
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Both primal and dual reductions	



This option determines whether primal reductions, dual reductions, or both, are performed during preprocessing. Possible values are:



*	No primal and dual reductions
*	Only primal reductions 
*	Only dual reductions
*	Both primal and dual reductions




In case the CPLEX presolver reports that a model is infeasible or unbounded, the solution reported by CPLEX cannot be interpreted. To aid analysis of an infeasible or unbounded declaration by the presolver, this option is provided that the user can set, so that the optimization can be rerun to make sure that the results reported by the presolver can be interpreted. If a model is declared by the presolver to be infeasible or unbounded and the user believes that it might be infeasible, this option can be set to 'Only primal reductions' by the user, and the presolver will only perform primal reductions. If the presolver still finds inconsistency in the model, it will be declared by the presolver to be infeasible, instead of infeasible or unbounded. Similarly, setting the option to 'Only dual reductions' means that if the presolver detects unboundedness in the model, it will be declared unambiguously to be unbounded.





This option is intended for diagnostic use, as turning off reductions will usually have a negative impact on the performance of the optimization algorithms in the normal (feasible and bounded) case.





If the model uses lazy constraints (either through a callback or a pool) then CPLEX turns off dual reductions.





**Learn more about** 

*	:ref:`CPLEX_User_Cuts_and_Lazy_Constraints` 
