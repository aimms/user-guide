

.. _Baron_Range_Reduction_-_Number_of_pr:


Number of probing problems
==========================



**Type** :	Integer	

**Range** :	{-2 .. 2100000000}	

**Default** :	-2	



This option specifies the number of probing problems allowed.



If the value equals -2 (the default) then BARON will automatically decide.



If the value equals -1 then there will be probing on all variables.



If the value equals n, n > 0, then there will be probing on n variables.



If the value equals 0, then there will be no range reduction by probing.



