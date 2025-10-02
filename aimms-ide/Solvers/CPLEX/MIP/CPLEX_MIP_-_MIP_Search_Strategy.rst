.. _option-CPLEX-mip_search_strategy:


MIP Search Strategy
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option sets the search strategy for a mixed integer program (MIP). Possible values are:

    *	Automatic
    *	Apply branch-and-cut
    *	Apply dynamic search


For many models, dynamic search finds feasible and optimal solutions more quickly than the conventional branch-and-cut algorithm.


An important drawback of the dynamic search algorithm is that it cannot be used in combination with some callbacks, if the
option **Use Generic Callbacks** is set to 'No'. The branch, candidate, cut, heuristic and lazy constraints callback procedures
will not be executed if 'Apply dynamic search' is chosen and the option **Use Generic Callbacks** is set to 'No'. However, the
callback procedures for incumbent, iterations, status change and time are still executed. See the section
:ref:`CPLEX_Threads_search_strat_and_callb`. If the generic callback implementation is used by CPLEX, activated by setting
the option **Use Generic Callbacks** to 'Yes', then all callback procedures (branch, candidate, cut, heuristic, incumbent,
iterations, lazy constraints, status change and time) can be used in combination with the dynamic search algorithm.


By default, CPLEX chooses whether to apply dynamic search or conventional branch-and-cut based on characteristics of the model
and the presence (or absence) of callbacks. If a branch, candidate, cut, heuristic or lazy constraints callback procedure is
present then CPLEX will choose the conventional branch-and-cut if the value of this option is 'Automatic'.


If the value of this option equals 'Apply branch-and-cut' then CPLEX will use only 1 thread if the option **Global Thread Limit**
equals its default value of 0 (unless the option **Stealth Mode** is set to 'Fast'). To let CPLEX use multiple threads you have
to set the **Global Thread Limit** to a value strictly larger than 1.


**Note** 

*	You might want to decrease the value of the general solvers option **Progress Time Interval** if the :ref:`aimmshelp12-progress_window` is no longer updated while solving your MIP model.
*	If dynamic search is used then AIMMS might become less responsive especially while solving the root node of the branch-and-bound tree.
*	The iterations and time callback procedures will be called less frequently in case dynamic search is used.


**Learn more about** 

*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`option-CPLEX-global_thread_limit` 
*	:ref:`option-AIMMS-progress_time_interval` 
*	:ref:`option-CPLEX-stealth_mode` 
*	:ref:`option-CPLEX-use_generic_callbacks` 

