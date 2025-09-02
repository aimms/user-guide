

.. _option-AIMMS-memory_bin_limit:


Memory Bin Limit
================



:Type:	Integer	
:Range:	{0 .. 4096}	
:Default:	1024	



The setting of this option determines which method of memory management will be used. If AIMMS requests an amount of memory smaller than Memory Bin Limit bytes, its own memory management system will be used, if this is not the case, the memory request will be handled by the operating system. 



The idea behind the AIMMS memory manager is that it is faster to allocate a lot of memory at once instead of allocating memory for each memory request. 



Setting this option to a high value will mean that allocating memory will go fast, but often has the side effect that more memory is allocated than AIMMS actually needs. 



**Note** 

*	You will have to restart AIMMS before a change in this option setting has effect.






