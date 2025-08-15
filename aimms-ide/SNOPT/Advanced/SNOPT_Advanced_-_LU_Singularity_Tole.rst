.. _SNOPT_Advanced_-_LU_Singularity_Tole:


LU Singularity Tolerance
========================



:Type:	Floating point number	
:Range:	[0,1] + {na}	
:Default:	na	



The LU density tolerance is used during LU factorization of the basis matrix. Columns of L and rows of U are formed one at a time, and the remaining rows and columns of the basis are altered appropriately. Ata any stage, if the density of the remaining matrix exceeds the value of this option, the Markowitz strategy for choosing pivots is terminated. The remaining matrix if factored by a dense LU procedure. Raising the density tolerance towards 1.0 may give slightly sparser LU factors, with a slight increase in factorization time.



The singularity tolerance helps guard against ill-conditioned basis matrices. When the basis is refactorized, the diagonal elements of U are tested as follows: if 



| Ujj | <= r  or  | Ujj | < r maxi | Uij | ``,`` 



the jth column of the basis is replaced by the corresponding slack variable. (This is most likely to occur after a restart, or at the start of a major iteration.)



In some cases, the Jacobian matrix may converge to values that make the basis exactly singular. (For example, a whole row of the Jacobian could be zero at an optimal solution.) Before exact singularity occurs, that basis could become very ill-conditioned and the optimization could progress very slowly (if at all). Setting a larger tolerance, say 1e-5, may help cause a judicious change of basis.



The default value of this option depends on the relative precision of the computer being used. On most computers the default equals 3.7e-11.



