.. _option-AIMMS-use_multiple_memory_managers:

Use Multiple Memory Managers
============================

:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	

When this option is switched on, high dimensional identifiers and generated mathematical programs get their own memory manager. 
A memory manager manages a collection of memory pools. 
By using multiple memory managers AIMMS 3.6 and upwards is able to defragment memory when 
identifiers are rebuild or emptied and when generated mathematical programs are discarded 
(by regenerating or by using the function GMP::Instance::Delete). 
Analysis of AIMMS' application test set proves that, except for a few pathalogical cases, 
the overhead incurred by using multiple memory managers is outweighed by the gain of defragmentation.

When this option is switched off the situation is returned to the AIMMS 3.5 and older systems.

Possible values are:

    *	On
    *	Off

**Learn more about** 

*	:any:`GMP::Instance::Delete`
