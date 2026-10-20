.. _option-ODHCPLEX-advanced_start:


Advanced Start
==============



:Type:	Selection
:Range:	The settings listed below
:Default:	Automatic



This option determines whether CPLEX uses advanced start information (a basis, start vector or MIP start) and how. Possible values are:

    *	Automatic (Default setting; for continuous models the behavior depends on the general solvers option **Accept Basis**.)
    *	Off (Do not use advanced start information.)
    *	Use advanced basis (Use the advanced start information as it is.)
    *	Crush advanced basis (First presolve the model and the advanced start information, then use it for the presolved model.)


**Continuous models**

*	Automatic: CPLEX uses the basis supplied by AIMMS if the general solvers option **Accept Basis** indicates that the basis should be
	accepted. Otherwise, CPLEX does not use advanced start information.
*	Off: CPLEX solves the model from scratch, with full presolve.
*	Use advanced basis: CPLEX starts the simplex algorithm from the currently loaded basis. If a basis is available only for the original,
	unpresolved model, or if CPLEX has a start vector rather than a simplex basis, then the simplex algorithm proceeds on the unpresolved
	model, i.e., the presolve is skipped.
*	Crush advanced basis: CPLEX first performs presolve on the model and on the basis or start vector, and then proceeds with optimization
	on the presolved problem. This setting can be particularly useful for solving fixed MIP models, where a start vector but no corresponding
	basis is available.

For continuous models solved with the barrier algorithm, the settings 'Use advanced basis' and 'Crush advanced basis' continue the
optimization from the last available barrier iterate.


**MIP models**

*	Use advanced basis: CPLEX continues with a partially explored MIP tree if one is available. If tree exploration has not yet begun,
	CPLEX uses the level values as a MIP start, if available.
*	Crush advanced basis: CPLEX retains the current incumbent (if there is one), re-applies presolve, and starts a new search from a new root.


**Which setting to use for continuous models**

Starting from an advanced basis is efficient if the basis is optimal or almost optimal, for example, if the same LP model is solved again
after small changes in bounds, right-hand sides or objective coefficients. That is why the default is 'Automatic'.

If consecutive LP models differ substantially, for example, in a rolling horizon approach, the basis can be a poor starting point. Because
the presolve is skipped when CPLEX starts from the basis ('Use advanced basis', or 'Automatic' if the basis is accepted), the solve can be
much slower than solving the model from scratch. In that case it is recommended to set this option to 'Off'. The setting 'Crush advanced
basis' applies the presolve, but does not help if the basis itself is a poor starting point.


**Note**

*	CPLEX also supports Multiple MIP Starts.
*	If this option is not switched off and if GMP functionality is used (e.g., :any:`GMP::Instance::Solve`), then CPLEX can resume a solve that was interrupted or hit a time, node or iteration limit.


**Learn more about**

*	:doc:`../../../Aimms/Options/Solvers General/Interface/Interface_-_Accept_Basis`
*	:doc:`../CPLEX MIP/ODH_XMIP_-_NumberofRepairAttempts`

