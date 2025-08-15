.. _XA_Advanced_-_Size_of_Smallest_El:


Size of Smallest Element
========================



**Type**:	Real	

**Range**:	[0,1]	

**Default**:	1e-12	



This option determines the smallest element that can be stored in the LU factors arrays. If the absolute value of a number is less than the value of this option then it is considered to be zero (0.0).



**Remark** 

Extreme caution should be exercised when changing the value of this option because of the overall effect on problem feasibility.



