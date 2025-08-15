.. _ODH-CPLEX_Advanced_-_Backtrack_Limit:


Backtrack Limit
===============



**Type**:	Integer	

**Range**:	{-1 .. 2100000000}	

**Default**:	-1



This option sets the maximum number of backtracks permitted in sub-model solves. Possible values are:




.. list-table::

   * - -1
     - Automatically determined (default)
   * - 0
     - Infinite
   * - >0
     - Use this value if a better solution is available




