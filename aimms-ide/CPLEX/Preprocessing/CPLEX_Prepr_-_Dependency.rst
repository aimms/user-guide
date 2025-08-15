.. _CPLEX_Prepr_-_Dependency:


Dependency
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The CPLEX preprocessor offers a "dependency checker" which strengthens problem reduction by detecting redundant constraints. Such reductions are usually most effective with the barrier optimizer. 



The activation of the "dependency checker" can be controlled by means of this option. If this option is set to "Check only at start of presolve", "Check only at end of presolve" or "Check at start and end of presolve", the dependency check will search for dependent rows during preprocessing. If this option is set to "No check", dependent rows will not be identified. For many models, eliminating the dependency check will speed up the preprocessing time, at the expense of not identifying dependent rows. Possible values are:



*	Automatic
*	No check
*	Check only at start of presolve
*	Check only at end of presolve
*	Check at start and end of presolve



