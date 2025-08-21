.. _option-XA-maximal_number_of_nodes:


Maximal Number of Nodes
=======================



:Type:	Integer	
:Range:	{0..2100000000}	
:Default:	2100000000	



This option determines the maximum number of branch and bound nodes. The value of 2100000000 has a special meaning; it defaults to 4000 plus the number of binary variables plus the square root of the number of integer columns.



**Remark** 

XA might face memory problems if the value of this option is very large.



