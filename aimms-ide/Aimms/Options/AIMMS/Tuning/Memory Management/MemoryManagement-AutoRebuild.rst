

.. _Options_MemoryManagement-AutoRebuild:


Auto Rebuild
============



Type:	Selection	

Range:	One of the settings listed below	

Default:	Off



When switching the option to on, AIMMS will check after each update of an identifier whether or not it is worthwhile to rebuild that identifier. It might be worth while to switch this option on when memory statistics report a high cardinality high dimensional identifier, which might contain a lot of unused memory.



The decision whether or not to rebuild, depends on the settings of the options Auto Rebuild Minimum Difference Absolute and Auto Rebuild Minimum Difference Relative.



Possible values are:



*	On
*	Off




**Learn more about** 

*	:ref:`Options_Memory_Management_-_AutoRebAbs` 
*	:ref:`Options_Memory_Management_-_AutoRebRel` 






