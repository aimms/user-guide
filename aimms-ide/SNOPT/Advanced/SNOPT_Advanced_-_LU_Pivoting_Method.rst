.. _option-SNOPT-lu_pivoting_method:


LU Pivoting Method
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Complete	



The basis factorization implements a Markowitz-type search for pivots that locally minimize the fill-in subject to a threshold pivoting stability criterion. The rook and complete pivoting options are more expensive than partial pivoting but are more stable and better at revealing rank, as long as the **LU Factor Tolerance**  is not too large (say t1 < 2.0).



When numerical difficulties are encountered, SNOPT automatically reduces the LU tolerances toward 1.0 and switches (if necessary) to rook or complete pivoting before reverting to the default or specified options at the next refactorization.



Possible values are:



*	Partial
*	Rook
*	Complete




**Learn more about** 

*	:ref:`option-SNOPT-lu_factor_tolerance`  






