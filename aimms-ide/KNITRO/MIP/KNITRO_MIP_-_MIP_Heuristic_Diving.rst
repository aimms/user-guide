.. _KNITRO_MIP_-_MIP_Heuristic_Diving:


MIP Heuristic Diving
====================



**Type** :	Bit Selection	

**Range** :	{-1..31}	

**Default** :	-1



This option specifies whether or not to enable the MIP diving heuristic. Possible values are:



*	-1 (automatic): Let Knitro determine automatically from :ref:`KNITRO_MIP_-_MIP_Heuristic_Strategy` 
*	0 (disable): Disable all diving heuristics
*	1 (bit 0): Enable fractional diving heuristic
*	2 (bit 1): Enable vector length diving heuristic
*	4 (bit 2): Enable coefficient diving heuristic
*	8 (bit 3): Enable linesearch diving heuristic
*	16 (bit 4): Enable guided diving heuristic




This option is a bit-valued option where various diving heuristics can be enabled by activating the corresponding bit value as described above. Setting this option to -1 will use an automatic setting and setting the value to 0 will disable all diving heuristics. Otherwise, set this parameter value to the sum of the values for the individual diving heuristics you wish to enable. For example, to enable only the “fractional” and “linesearch” diving heuristics, you would set this option value to 9 (summing 1 for fractional and 8 for linesearch).





**Learn more about** 

*	:ref:`KNITRO_MIP_-_MIP_Heuristic` 
*	:ref:`KNITRO_MIP_-_MIP_Heuristic_Strategy` 



