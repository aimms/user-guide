.. _option-CPLEX-use_generic_callbacks:


Use Generic Callbacks
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines whether CPLEX should use generic callback procedures, as introduced in CPLEX 12.9, for mixed integer optimization. Possible values are:



    *	No
    *	Yes




Callback procedures (or callbacks) allow you to monitor closely and to guide the behavior of the CPLEX optimizers. In particular, callbacks allow user code to be executed regularly during an optimization run. Examples are callback procedures for branch, candidate, cut, heuristic or lazy constraints. Callback procedures are also used by AIMMS to update the information in the Progress Window during a solve. These callback procedures have been implemented using generic callbacks and legacy callbacks. This option selects which implementation will be used.





The more recent implementation of generic callbacks, contrast legacy callbacks, such as informational callbacks and control callbacks (already familiar in CPLEX) with the more recent implementation of generic callbacks. Legacy callbacks were designed when CPLEX was a branch-and-bound or branch-and-cut solver. Consequently, those legacy callbacks were designed to monitor and control a branch-and-bound or branch-and-cut search. This design implies that those legacy callbacks assume a branch-and-bound or branch-and-cut context throughout their invocation. For example, such legacy callbacks usually assume a "current node" context. This assumption is one of the reasons that the legacy callbacks are incompatible with dynamic search.





Over time, CPLEX has evolved and now executes more sophisticated strategies than straightforward branch-and-bound or branch-and-cut, although that strategy is still at the core of the solver. Dynamic search and other features have been added to CPLEX to solve models faster. The generic callback is compatible with all these new features since it does not assume a strictly branch-and-bound or branch-and-cut perspective in the solution process. It only assumes a generic search for an optimal solution. As a consequence, it does not allow user control of the the branch-and-bound or branch-and-cut process in as much detail as the legacy callbacks do. Such low-level control, however, is not usually required. The degree of control offered by the generic callback is more high level, yet frequently that degree of control is all that is needed.





The usage of generic callback has several benefits:





*   It is compatible with dynamic search, as controlled by the option **MIP Search Strategy**.
*   It does not require disabling any MIP features. 
*   It monitors progress as well as guides the search. 
*   It does not implicitly change the number of threads that CPLEX uses (which is controlled by the option **Global Thread Limit** ).
*   Using an empty generic callback will yield the same solution path as using no generic callback. (This convention is not true for CPLEX legacy callbacks.) Of course, invoking an empty callback incurs some overhead, so a run with an empty callback will be slightly slower than a run without any callback, but the solution path will still be the same. 




The usage of generic callback also has some disadvantages:





*   It does not provide progress information while solving the root node of the branch-and-bound tree.
*   The solve cannot be interrupted while CPLEX is solving the root node of the branch-and-bound tree.
*   It does not support the branch callback. If a branch callback is installed then legacy callbacks will be used even if this option is set to 'Yes'.
*   It does not report the number of nodes left. This implies that the 'Left' field in the Progress Window will remain at 0, and the function GMP::SolverSession::GetNodesLeft will always return 0.
*   It does not report the node objective. This implies that the function GMP::SolverSession::GetNodeObjective will always return 'na'.




**Note** 

*	For solving LP, QP, QCP or RMIP models legacy callbacks will be used even if this option is set to 'Yes'. This also holds for the postsolve step of a MIP model (because then an LP model is solved).
*	Generic callbacks will be used for solving multi-objective optimization models even if this option is set to 'No', also for multi-objective LP models. As a consequence, when solving a multi-objective LP model CPLEX cannot be interrupted and no progress information is provided during the solve.
*	The behavior of CPLEX will be opportunistic if this option is set to 'Yes' and if a branch, candidate, cut or lazy constraint callback is installed, the option Global Thread Limit is set to a value greater than 1, and the option Parallel Mode is set to 'deterministic'. (The behavior will also be opportunistic in this situation if legacy callbacks are used.) If no callback or only a heuristic callback is installed then the behavior will be deterministic.
*	Searching for a global optimum for a QP model is considered as mixed integer optimization because in that case CPLEX first changes the problem type to MIQP. Therefore, for a QP model, if this option is set to 'Yes' and the option **Solution Target**  is set to 'Search for global optimum' then generic callbacks will be used.




**Learn more about** 

*	:any:`GMP::SolverSession::GetNodeObjective`
*	:any:`GMP::SolverSession::GetNodesLeft`
*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`option-CPLEX-global_thread_limit` 
*	:ref:`option-CPLEX-mip_search_strategy` 
*	:ref:`option-CPLEX-parallel_mode` 
*	:ref:`option-AIMMS-postsolve` 
*	:ref:`option-CPLEX-solution_target` 



