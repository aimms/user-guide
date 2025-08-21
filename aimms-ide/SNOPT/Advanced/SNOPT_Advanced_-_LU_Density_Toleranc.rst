.. _option-SNOPT-lu_density_tolerance:


LU Density Tolerance
====================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0.6	



The LU density tolerance is used during LU factorization of the basis matrix. Columns of L and rows of U are formed one at a time, and the remaining rows and columns of the basis are altered appropriately. At any stage, if the density of the remaining matrix exceeds the value of this option, the Markowitz strategy for choosing pivots is terminated. The remaining matrix if factored by a dense LU procedure. Raising the density tolerance towards 1.0 may give slightly sparser LU factors, with a slight increase in factorization time.



