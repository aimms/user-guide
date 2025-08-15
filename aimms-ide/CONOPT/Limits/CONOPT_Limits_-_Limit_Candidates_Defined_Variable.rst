.. _CONOPT_Limits_-_Limit_Candidates_Defined_Variable:

Limit on Candidates for Defined Variable
========================================



:Type:	Integer	
:Range:	{0..:ref:`Miscellaneous_Maxint` }	
:Default:	2	



When there is more than one candidate that can be selected as a defined variable in a particular constraint, CONOPT tries to select the most appropriate in order to select as many defined variables as possible. However, to avoid too much arbitrariness this is only attempted if there are not more than **Limit on Candidates for Defined Variable**  candidates.



**Note** 

*	Defined variables are identified from constraints of the type x(i) = f(x) where x(i) is free or implied free.
