.. _option-KNITRO-mip_branching_rule:


MIP Branching Rule
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which branching rule to use for the MIP branch and bound procedure. Possible values are:



    *	Automatic
    *	Most fractional
    *	Pseudo-cost
    *	Strong branching




Setting 'Most fractional' implies using the most fractional (most infeasible) branching.





In case of strong branching, the options **Strong Branching Candidates Limit**, **Strong Branching Iteration Limit**  and **Strong Branching Level**  can be used for further control of strong branching procedure).





**Learn more about** 

*	:ref:`option-KNITRO-strong_branching_candidates_limit`  
*	:ref:`option-KNITRO-strong_branching_iteration_limit`  
*	:ref:`option-KNITRO-strong_branching_level`  
