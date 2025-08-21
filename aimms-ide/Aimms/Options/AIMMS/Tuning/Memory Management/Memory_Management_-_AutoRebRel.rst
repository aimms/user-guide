

.. _option-AIMMS-auto_rebuild_minimum_difference_relative:


Auto Rebuild Minimum Difference Relative
========================================



:Type:	Floating Point Number	
:Range:	[0.01, 0.99]	
:Default:	0.75	



Together with the option Auto Rebuild Minimum Difference Absolute this option determines whether or not to rebuild an identifier. If the total memory used by the identifier memory manager minus the memory used by the ordered view of that identifier divided by the total memory used by the identifier memory manager is larger than the value of this option, AIMMS will rebuild the identifier.



**Learn more about** 

*	:ref:`option-AIMMS-auto_rebuild`  
*	:ref:`option-AIMMS-auto_rebuild_minimum_difference_absolute` 









