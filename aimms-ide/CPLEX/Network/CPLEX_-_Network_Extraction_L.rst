.. _option-CPLEX-network_extraction_level:


Network Extraction Level
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Try reflection scaling	



This option establishes the level of network extraction for network simplex optimizations when **LP Method**  is set to "Network + Primal"or "Network + Dual". The default value is suitable for recognizing commonly used modeling approaches when representing a network problem within an LP formulation. Possible values are:



    *	Extract pure network only
    *	Try reflection scaling
    *	Try general scaling




**Learn more about** 

*	:ref:`option-CPLEX-lp_method` 



