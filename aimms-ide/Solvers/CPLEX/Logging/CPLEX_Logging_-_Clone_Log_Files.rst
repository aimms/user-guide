.. _option-CPLEX-clone_log_files:


Clone Log Files
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic



This option specifies whether CPLEX clones the log files of nodes during parallel or concurrent optimization. When you use parallel or concurrent CPLEX, this feature makes it more convenient to check node logs when you use more than one thread to solve models. For parallel optimization on N threads, for example, turning on this parameter creates N logs, clone[0].log through clone[N-1].log. This feature is available only during concurrent optimization and mixed integer programming (MIP) optimization. Possible values are:



    *	Off
    *	Automatic
    *	On




The concurrent optimizer is described in the section :ref:`CPLEX_Parallel_Concurrent_Optimizer`. It can be enabled by setting the option **LP Method**. The amount of information printed to the clone log files is controlled by the options **Barrier Display**  and **Simplex Display**.





The parallel MIP optimizer is controlled by the option **Global Thread Limit**. The amount of information printed to the clone log files is controlled by the options **MIP Display**  and **MIP Interval**.





The clone log files are written in the project folder (and not to the log directory).





**Learn more about** 

*	:ref:`option-CPLEX-barrier_display` 
*	:ref:`option-CPLEX-global_thread_limit`  
*	:ref:`option-CPLEX-lp_method` 
*	:ref:`option-CPLEX-mip_display` 
*	:ref:`option-CPLEX-mip_interval` 
*	:ref:`CPLEX_Parallel_Concurrent_Optimizer` 
*	:ref:`option-CPLEX-simplex_display` 
