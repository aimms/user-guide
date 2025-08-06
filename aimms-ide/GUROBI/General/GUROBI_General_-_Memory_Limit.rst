.. _GUROBI_General_-_Memory_Limit:


Memory Limit
============



**Type** :	Floating point number	

**Range** :	[0,1e100]	

**Default** :	1e100



This option limits the total amount of memory (in GB, i.e., 109 bytes) available to Gurobi. If more is needed, Gurobi will fail with an out-of-memory error.



Note that it is not possible to retrieve solution information after an error termination. Thus, the behavior of this option is different from that of the option **Soft Memory Limit** , where if the solver will terminate then solution information will still be available.



One advantage of using this option rather than the similar **Soft Memory Limit**  is that this ootion is checked after every memory allocation, so Gurobi will terminate at precisely the point where the limit is exceeded.



Memory usage is also tracked across all threads. One consequence of this is that termination may be non-deterministic for multi-threaded runs.



**Note** 

*	If the GMP::Solver::InitializeEnvironment procedure is used to initialize Gurobi then this option cannot be set using the Option Tree. Instead you should use the procedure GMP::Solver::SetEnvironmentDoubleParameter with "MemLimit" as argument.




**Learn more about** 

*	:ref:`GUROBI_General_-_Soft_Memory_Limit`  



