.. _ODH-CPLEX_XLogging_-_Clone_Log_Files:


Clone Log Files
===============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic



This option specifies whether CPLEX clones the log files of nodes during parallel or concurrent optimization. When you use parallel or concurrent CPLEX, this feature makes it more convenient to check node logs when you use more than one thread to solve models. For parallel optimization on N threads, for example, turning on this parameter creates N logs, clone[0].log through clone[N-1].log. This feature is available only during concurrent optimization and mixed integer programming (MIP) optimization. Possible values are:



*	Off
*	Automatic
*	On




The amount of information printed to the clone log files is controlled by the options **Barrier Display**  and **Simplex Display** .





The parallel MIP optimizer is controlled by the option **Global Thread Limit** . The amount of information printed to the clone log files is controlled by the options **MIP Display**  and **MIP Interval** .





The clone log files are written in the project folder (and not to the log directory).





**Learn more about** 

*	:ref:`ODH-CPLEX_XLogging_-_Barrier_Display` 
*	:ref:`ODH-CPLEX_XPar_-_GlobalThreadLimit`  
*	:ref:`ODH-CPLEX_XLogging_-_MIP_Display` 
*	:ref:`ODH-CPLEX_XLogging_-_MIP_Interval` 
*	:ref:`ODH-CPLEX_XLogging_-_Simplex_Display` 
