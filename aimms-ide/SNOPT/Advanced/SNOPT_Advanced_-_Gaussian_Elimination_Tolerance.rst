.. _SNOPT_Advanced_-_Gaussian_Elimination_Tolerance:


Gaussian Elimination Tolerance
==============================



**Type**:	Floating point number	

**Range**:	[1e-13,1e-5] + {na}	

**Default**:	na	



Tolerance used during Gaussian elimination. If the absolute value of an element is smaller than the value of this option then it is handled as 0.



The default value of this option depends on the relative precision of the computer being used. It is equal to eps^0.8 where eps is the machine precision.



