

.. _Baron_Local_Search_Heuristic_-_Numbe:


Number of preprocessing searches
================================



**Type**:	Integer	

**Range**:	{-2 .. 2100000000}	

**Default**:	-2	



This option specifies the number of local searches done in NLP preprocessing. The first one begins with the user-specified starting point as long as it is feasible. Subsequent local searches are done from randomly generated starting points.



If this option is set to −1, local searches in preprocessing will be done until proof of globality or the time limit is reached.



If this option is set to −2, BARON decides the number of local searches in preprocessing based on problem and NLP solver characteristics.

