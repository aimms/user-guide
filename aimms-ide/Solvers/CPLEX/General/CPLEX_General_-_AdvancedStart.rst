.. _option-CPLEX-advanced_start:


Advanced Start
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether advanced start information should be used and how. Possible values are:

    *	Automatic (Default setting; behavior depends on the setting of the general solvers option **Accept Basis**.)
    *	Off (Do not use advanced start information.)
    *	Use advanced basis (In case of a continuous model, CPLEX will use an advanced basis supplied by the user. In case of MIP, CPLEX will use the level values as start values or continue exploring the MIP tree if one is available.)
    *	Crush advanced basis (In case of a continuous model, CPLEX will crush an advanced basis or starting vector supplied by the user. In case of MIP, CPLEX will use the level values as start values or continue exploring the MIP tree if one is available.)


If set to 'Use advanced basis' or 'Crush advanced basis', this option indicates that CPLEX should use advanced starting
information when optimization is initiated.


For MIP models, setting 'Use advanced basis' will cause CPLEX to continue with a partially explored MIP tree if one is available.
If tree exploration has not yet begun, this setting specifies that CPLEX should use a loaded MIP start, if available. Setting
'Crush advanced basis' retains the current incumbent (if there is one), re-applies presolve, and starts a new search from a new root.


For continuous models solved with the simplex algorithm, setting 'Use advanced basis' will use the currently loaded basis. If a basis
is available only for the original, unpresolved model, or if CPLEX has a start vector rather than a simplex basis, then the simplex
algorithm will proceed on the unpresolved model. With setting 'Crush advanced basis', CPLEX will first perform presolve on the model
and on the basis or start vector, and then proceed with optimization on the presolved problem. Setting 'Crush advanced basis' can be
particularly useful for solving fixed MIP models, where a start vector but no corresponding basis is available.


For continuous models solved with the barrier algorithm, settings 'Use advanced basis' or 'Crush advanced basis' will continue optimization
from the last available barrier iterate.


For continuous models with setting 'Automatic', CPLEX will use an advanced basis supplied by the user if the value of the general solvers
option **Accept Basis** indicates that the basis should be accepted, and CPLEX will not use advanced start information if the value of the
**Accept Basis** indicates that the basis should be rejected.


**Note** 

*	CPLEX also supports :ref:`CPLEX_Multiple_MIP_Starts`.
*	If this option is not switched off and if GMP functionality is used (e.g., :any:`GMP::Instance::Solve`), then CPLEX can resume a solve that was interrupted or hit a time, node or iteration limit.


**Learn more about** 

*	:ref:`option-AIMMS-accept_basis`  
*	:ref:`option-CPLEX-number_of_repair_attempts`  
*	:ref:`CPLEX_Multiple_MIP_Starts` 

