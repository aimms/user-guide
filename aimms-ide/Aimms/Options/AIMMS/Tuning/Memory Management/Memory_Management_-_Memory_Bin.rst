

.. _Options_Memory_Management_-_Memory_Bin:


Memory Bin Allocation Size
==========================



**Type**:	Integer	

**Range**:	{ 1024 … 33554432 }	

**Default**:	1048576	



When AIMMS requests a block of memory smaller than Memory Bin Limit bytes for the first time, a block of memory with the size Memory Bin Allocation Size bytes will be allocated (within AIMMS this is called a Large Block). This Large Block will be subdivided into smaller Bins, each with size Memory Bin Size. At this first memory request the first Bin will also be subdivided; it will be divided into a series of so-called Small Blocks. All Small Blocks within a single Bin have the same size, which is determined by the amount of memory requested and the setting of the option Memory Bin Resolution.



If additional memory requests are of the Small Block used in the first Bin, a Small Block in this Bin will be assigned to the request. If not, a new Bin is subdivided into Small Blocks with the size of the request. If no free Bins with the requested size van be allocated in the current Large Block, a completely new Large Block will be allocated.



The setting of this option determines how large the large blocks are that are allocated by the AIMMS memory manager.



The higher the setting of this option, the faster the AIMMS memory manager will be. Using a high value however might also lead to more memory being allocated than is actually needed. In case you think your model might benefit from a different setting you can set the option Memory Statistics to On and use the function MemoryStatistics to compare the results.



**Note** 

*	You will have to restart AIMMS before a change in this option setting has effect.




**Learn more about** 

*	:ref:`Options_Memory_Management_-_Memory_Bi1`  
*	:ref:`Options_Memory_Management_-_Memory_Bi3`  
*	:ref:`Options_Memory_Management_-_Memory_Bi2`  
*	:ref:`Options_Memory_Management_-_Memory_Sta`  
*	:any:`MemoryStatistics`






