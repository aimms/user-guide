

.. _Options_Memory_Management_-_AutoRebAbs:


Auto Rebuild Minimum Difference Absolute
========================================



Type:	Integer	

Range:	{ 1048576 … :ref:`Miscellaneous_Maxint`  }	

Default:	104857600	



Together with the option Auto Rebuild Minimum Difference Relative this option determines whether or not to rebuild an identifier. If total memory used by the identifier memory manager minus the memory used by the ordered view of that identifier is larger than the value of this option, AIMMS will rebuild the identifier.



**Learn more about** 

*	:ref:`Options_MemoryManagement-AutoRebuild`  
*	:ref:`Options_Memory_Management_-_AutoRebRel`  









