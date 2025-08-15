.. _KNITRO_MIP_-_MIP_Heuristic_Large_Neighborhood_Search:

MIP Heuristic Large Neighborhood Search
=======================================



:Type:	Bit Selection	
:Range:	{-1..3}	
:Default:	-1



This option specifies whether or not to enable the MIP large neighborhood search heuristics. Possible values are:



*	-1 (auto): Let Knitro determine automatically from :ref:`KNITRO_MIP_-_MIP_Heuristic_Strategy` 
*	0 (disable): Disable all large neighborhood search heuristics
*	1 (bit 0): Enable relaxation enforced neighborhood search (RENS) heuristic
*	2 (bit 1): Enable relaxation induced neighborhood search (RINS) heuristic




Knitro considers the bit values of this parameter. For example, if this parameter is set to 3, bit 0 and bit 1 are equal to 1 and, as a result, both RENS and RINS heuristics are enabled. If this parameter is set to 2, only RINS heuristic is enabled.





**Learn more about** 

*	:ref:`KNITRO_MIP_-_MIP_Heuristic` 
*	:ref:`KNITRO_MIP_-_MIP_Heuristic_Strategy` 



