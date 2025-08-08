

.. _Options_MemoryManagement-Rebuild_before_solve:


Rebuild Before Solve
====================



Type:	Selection	

Range:	One of the settings listed below	

Default:	On	



Adding and removing elements in identifiers may cause the memory in those identifiers to become fragmented and thus occupying an unnecessary amount of memory. By rebuilding these identifiers, this memory is reclaimed. This memory could be reused at the start of a solve statement. When this option is switched on at the start of the solve statements, selected identifiers are rebuilt in order to reclaim memory that can be reused in the generation of mathematical programs. The identifiers selected are those that have sufficient amount fragmented memory to warrant the rebuilding of the data trees.



Possible values are:



*	On
*	Off




**Learn more about** 

*	:ref:`rebuild` 







**Note** 





The difference between the rebuilding done at the beginning of the SOLVE statement and the rebuild statement is that the REBUILD statement also considers the permutations of the data trees as memory fragmentation whilst the rebuild at the start of the SOLVE statement considers these permutations to be memory in use.




