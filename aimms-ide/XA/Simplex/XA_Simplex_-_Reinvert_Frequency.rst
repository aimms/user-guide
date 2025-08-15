.. _XA_Simplex_-_Reinvert_Frequency:


Reinvert Frequency
==================



**Type**:	Integer	

**Range**:	{0..2100000000}	

**Default**:	40	



The value of this option determines the number of iterations (pivots) after which the basis is factorized based upon the current columns in the basis and all LU pivoting factors are removed. Reducing the number of pivots before this so-called 're-inversion' usually reduces the number of iterations to solve a problem but at the expense of performing more basis inversions that cost more CPU time.



