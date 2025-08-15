.. _CPOPT_Logging_-_Mod_file:


Mod file
========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



This option can be used to generate a mod file of the current model loaded. The model is written to a file called cpoddddd.mod, where ddddd denotes a 5 digit sequence number. A mod file can be read by IBM ILOG CPLEX Optimization Studio. Possible values are:



*	Off
*	On




The mod file cannot be printed in the following situations:





*   One of the schedule domains is non-contiguous
*   The value of option **Cardinality Encoding**  equals 'Distribute'
*   The value of option **Sequence Encoding**  unequals 'Count'




**Learn more about** 

*	:ref:`CPOPT_Inference_-_Cardinality_encoding` 
*	:ref:`CPOPT_Logging_-_Mod_file_write_constraint_name` 
*	:ref:`CPOPT_Inference_-_Sequence_encoding` 
