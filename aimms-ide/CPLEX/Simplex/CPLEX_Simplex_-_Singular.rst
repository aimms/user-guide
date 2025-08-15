.. _CPLEX_Simplex_-_Singular:


Singular
========



**Type**:	Integer	

**Range**:	{0 .. 2100000000}	

**Default**:	10	



This option restricts the number of times CPLEX will attempt to repair the basis when singularities are encountered. Once the limit is exceeded, CPLEX replaces the current basis with the best factorizable basis that has been found.



