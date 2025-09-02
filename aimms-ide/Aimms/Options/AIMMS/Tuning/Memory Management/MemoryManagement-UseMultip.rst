.. _option-AIMMS-use_multiple_memory_managers:

Use Multiple Memory Managers
============================

:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	

When this option is switched on, high dimensional identifiers and generated mathematical programs get their own memory manager. 
A memory manager manages a collection of memory pools. 
By using multiple memory managers AIMMS is able to defragment memory when 
identifiers are rebuild or emptied and when generated mathematical programs are discarded 
(by regenerating or by using the function :any:`GMP::Instance::Delete`). 
Analysis of AIMMS' application test set proves that, except for a few pathalogical cases, 
the overhead incurred by using multiple memory managers is outweighed by the gain of defragmentation.

Possible values are:

    *	On
    *	Off

**Learn more about** 

*	:any:`GMP::Instance::Delete`
