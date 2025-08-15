.. _CONOPT_Limits_-_Maximal_Hessian_Dim:

Maximal Hessian Dimension
=========================



:Type:	Integer	
:Range:	{5..:ref:`Miscellaneous_Maxint` }	
:Default:	500	



If the number of superbasics exceeds the value of this option, CONOPT will no longer use the BFGS algorithm but will switch to a steepest descent approach, independent of the degree of nonlinearity of the model. If the value of this option is increased beyond its default value, the default memory allocation may not be sufficient. You may have to change the option solver workspace. You should try increasing the value of this optionif CONOPT performs many iterations in Phase 4 with the number of superbasics (NSB) larger than the value of this optionand without much progress. The new value should, in this case, be larger than the number of superbasics.



