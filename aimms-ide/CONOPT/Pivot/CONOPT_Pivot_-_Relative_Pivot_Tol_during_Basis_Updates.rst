.. _CONOPT_Pivot_-_Relative_Pivot_Tol_during_Basis_Updates:

Relative Pivot Tolerance during Basis Updates
=============================================



**Type**:	Floating point number	

**Range**:	[3e-13,0.001]	

**Default**:	1e-7	



This option specifies the relative pivot tolerance during basis updates. During basis changes CONOPT attempts to use cheap updates of the LU-factors of the basis. A pivot is considered large enough relative to the alternatives in the column if its absolute value is at least RPT * the other element, where RPT denotes the value of this option. Smaller values of RPT will allow sparser basis updates but may cause accumulation of larger numerical errors.



**Learn more about** 

*	:ref:`CONOPT_Pivot_-_Relative_Pivot_Tol`  
