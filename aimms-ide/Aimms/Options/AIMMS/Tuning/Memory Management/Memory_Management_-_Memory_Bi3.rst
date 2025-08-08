

.. _Options_Memory_Management_-_Memory_Bi3:


Memory Bin Size
===============



Type:	Selection	

Range:	One of the settings listed below	

Default:	8 K	



When AIMMS requests a block of memory smaller than Memory Bin Limit bytes for the first time, a block of memory with the size Memory Bin Allocation Size bytes will be allocated (within AIMMS this is called a Large Block). This Large Block will be subdivided into smaller Bins, each with size Memory Bin Size. At this first memory request the first Bin will also be subdivided; it will be divided into a series of so-called Small Blocks. All Small Blocks within a single Bin have the same size, which is determined by the amount of memory requested and the setting of the option Memory Bin Resolution.



If additional memory requests are of the Small Block used in the first Bin, a Small Block in this Bin will be assigned to the request. If not, a new Bin is subdivided into Small Blocks with the size of the request. If no free Bins with the requested size van be allocated in the current Large Block, a completely new Large Block will be allocated.



The setting of this option determines how large the Bins are that are made by the memory manager.



Depending on the setting of this option, the AIMMS memory manager might be more efficient or faster. This depends on the model and it is not possible to predict the outcome in advance. In case you think your model might benefit from a different setting you can set the option Memory Statistics to On and use the function MemoryStatistics to compare the results.



Possible values are:



*	1 K
*	2 K
*	4 K
*	8 K
*	16 K
*	32 K
*	64 K




**Note** 

*	You will have to restart AIMMS before a change in this option setting has effect.




**Learn more about** 

*	:ref:`Options_Memory_Management_-_Memory_Bi1`  
*	:ref:`Options_Memory_Management_-_Memory_Bin`  
*	:ref:`Options_Memory_Management_-_Memory_Bi2`  
*	:ref:`Options_Memory_Management_-_Memory_Sta`  
*	:any:`MemoryStatistics`






