.. _option-ODHCPLEX-node_file:


Node File
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	In memory and compressed	



This option is used when the **Working Memory Limit**  has been exceeded by the size of the tree. Possible values are:



*	None
*	In memory and compressed
*	On disk
*	On disk and compressed




If the node file parameter is set to 'None' when the tree memory limit is reached, optimization is terminated. Otherwise, a group of nodes is removed from the in-memory set as needed. If the value is 'In memory and compressed' (the default), then a very fast compression algorithm is used on the nodes to try to conserve memory, without resorting to write the node files to disk. At settings 'On disk' and 'On disk and compressed', the node files are transferred to disk, in uncompressed and compressed form respectively, and CPLEX actively manages which nodes remain in memory for processing.





**Learn more about** 

*	:ref:`option-ODHCPLEX-working_memory_limit` 



