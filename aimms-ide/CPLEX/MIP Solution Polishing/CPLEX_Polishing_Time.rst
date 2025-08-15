.. _CPLEX_Polishing_Time:


Polishing Time
==============



**Type**:	Floating point number	

**Range**:	[0,inf)	

**Default**:	1e75	



This option sets the amount of time (in seconds) to spend during a normal mixed integer optimization before CPLEX starts to polish a feasible solution. During solution polishing, CPLEX applies its effort to trying to improve the best feasible solution. Polishing can yield better solutions in some situations. The default value (1e75 seconds) is such that CPLEX does **not**  start solution polishing by default.



As an example of how to manage time spent polishing a feasible solution, suppose the user wants to solve a problem by spending 100 seconds in branch & cut and an additional 200 seconds in polishing. Then the user should apply the following commands:




.. list-table::

   * - 1.
     - Set the general time limit as controlled by the general solvers option **Time Limit**  to 300.0 seconds. In CPLEX, this option controls the total time spent in branch & cut plus solution polishing.
   * - 2.
     - Establish a starting condition for solution polishing by setting this option to 100.0 seconds. This option controls the time spent in branch & cut before CPLEX switches to polishing.
   * - 3.
     - Call the optimizer.




If CPLEX does not find a solution in the first 100 seconds, then this procedure continues branch & cut until it finds a solution, and afterwards switches to polishing. This procedure guarantees that CPLEX spends at most 300 seconds on the model and that CPLEX applies polishing if a solution is found during that time.



**Note** 

*	Branching priorities have a limited effect on solution polishing. In solution polishing, the usual branch and bounding continues, so the new nodes that are created during solution polishing will be created according to the priorities. However, the solution polishing process itself which is performed at each node does not pay any attention to the priorities.
*	The option **Polishing Time Deterministic** limits the amount of time spent in deterministic ticks (rather than seconds).




**Learn more about** 

*	:ref:`CPLEX_Polishing_Time_Deterministic`  
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
