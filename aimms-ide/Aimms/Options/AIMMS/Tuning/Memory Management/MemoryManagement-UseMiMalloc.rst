.. _option-AIMMS-memory_use_mimalloc:

Memory Use MiMalloc
===================

:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	Off

With this option enabled, AIMMS will use *mimalloc* (by Microsoft) as the underlying memory allocation system (instead of *dlmalloc*).
Tests have shown that *mimalloc* may initially use a bit more memory, but for long-running apps the memory consumption is much more stable.
With *dlmalloc* (the default), the total 'memory in use' sometimes seems to be constantly growing (due to memory fragmentation).

Possible values are:

    *	On
    *	Off

**Note** 

*	You will have to restart AIMMS before a change in this option setting has effect.

