

.. _option-AIMMS-eliminate_nonvar_columns:


Eliminate Nonvar Columns
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option provides an override to explicitly retain those columns in the generated matrix of a mathematical program which would normally be eliminated by the matrix generation algorithm of AIMMS.

 

You should only need to use this option if you, for example, want such columns to explicitly appear in the constraint listing.



The matrix generation algorithm will decide whether or not to generate a column for a reference to a variable in the formulation of a constraint that occurs in the declaration of a mathematical program, by consecutively checking the following set of rules below. Note that the option **Eliminate Nonvar Columns**  only has an impact on a few rules!



1.	AIMMS will never generate matrix columns for 

-	a symbolic variable that is not contained in the variable set of a mathematical program,

-	an index tuple of a symbolic variable that is not contained in its domain (i.e. does not satisfy the domain restriction),

-	a variable for which one of the indices in the domain refers to a HORIZON, and the corresponding element in the HORIZON falls outside the planning interval of the HORIZON.

2.	If the NONVAR STATUS attribute of a variable (or the .nonvar suffix) assumes a value 

-	< 0, then AIMMS will always generate a column,

-	> 0, then AIMMS will only generate a column if the option **Eliminate Nonvar Columns**  is switched off.

In these cases, both bounds of the generated columns will be set equal to the level value of the associated variables prior to generating. 

3.	If the NONVAR STATUS attribute is equal to 0, and the lower and upper bound of a variable are equal, then AIMMS will only generate a column if the option **Eliminate Nonvar Columns**  is switched off. 

4.	In all other cases AIMMS will generate a column in the matrix.



Possible values are:



*	On
*	Off
*	Automatic




The value 'Automatic' means that the option is set to 'On' unless the mathematical program type equals COP or CSP, in which case it will be set to 'Off'.





**Note** 


The new implementation of the matrix generation (introduced in version 24.6) will NOT use this option. It only looks at the rules mentioned above. If you want to programmatically change the nonvar status you can also (instead of using this option) use a scalar parameter (with values 0, -1, or 1) to assign to the nonvar property or .nonvar suffix.








**Remark** 


Stochastic variables are always generated, expect for rule 1, even if the .nonvar suffix is set to a value > 0 and the option **Eliminate Nonvar Columns**  is switched on. That is, using





	Y.Stochastic(sc).nonvar := 1;





or





	Y.Stochastic(sc).nonvar := -1;





makes no difference. In both cases the lower and upper bound of Y.Stochastic(sc) will be set equal to the level value.

