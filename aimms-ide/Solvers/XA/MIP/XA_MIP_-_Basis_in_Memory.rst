.. _option-XA-basis_in_memory:


Basis in Memory
===============



:Type:	Integer	
:Range:	{0..2100000000}	
:Default:	0	



Maximum number of integer basis to maintain in memory. The size of each integer basis is two bits times the number of columns and rows. The default value of 0 corresponds to a setting, in which all integer basis are stored if sufficient memory is available. If this is not the case, then space for 100 integer basis is reserved. This number can affect the performance of solving MIPs; it is reported in the statistics report.



