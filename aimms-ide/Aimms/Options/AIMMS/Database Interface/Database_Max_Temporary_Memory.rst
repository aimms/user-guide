

.. _Options_Database_Max_Temporary_Memory:


Database Max Temporary Memory
=============================



**Type**:	Integer	

**Range**:	{1..:ref:`Miscellaneous_Maxint`  }	

**Default**:	64	



This option determines the maximum amount of temporary memory (in megabytes) the database connector will use for executing certain database operations. 



AIMMS uses this option to determine performance versus memory usage. When your read or write statements from/to databases are performing bad, you might experiment with increasing this value. When you feel the database connector is using too much memory, you can lower this value (to a minimum of 1 megabyte).

