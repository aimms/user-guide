.. _option-CBC-trust_pseudo_costs:


Trust Pseudo Costs
==================



:Type:	Integer	
:Range:	{-3 .. 2000000}	
:Default:	5	



This option sets the number of branches before we trust pseudo-costs. Using strong branching computes pseudo-costs. After this many times for a variable we just trust the pseudo-costs and do not do any more strong branching.



**Learn more about** 

*	:doc:`CBC_MIP_-_Strong_branching` 
