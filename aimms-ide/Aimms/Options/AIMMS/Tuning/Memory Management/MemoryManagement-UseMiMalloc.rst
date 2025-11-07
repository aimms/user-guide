.. _option-AIMMS-memory_use_mimalloc:

Use MiMalloc
============

:Type:	Selection	
:Range:	{ On , Off }
:Default:	Off	

With this option enabled, AIMMS will use MiMalloc (by Microsoft) as the underlying memory allocation system (instead of dlMalloc).
Tests have shown that MiMalloc may initially use a bit more memory, but for long-running apps the memory consumption is much more stable.
With dlMalloc (the default), the total 'memory in use' sometimes seems to be constantly  growing (due to memory fragmentation).

Note: if you change this option, you must close and restart AIMMS to use the new setting.


