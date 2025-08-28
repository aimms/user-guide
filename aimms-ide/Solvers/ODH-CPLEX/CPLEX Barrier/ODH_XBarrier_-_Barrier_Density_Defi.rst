.. _option-ODHCPLEX-barrier_density_definition:


Barrier Density Definition
==========================



:Type:	Integer	
:Range:	{1 .. 2100000000}	
:Default:	0	



This option is used in the recognition of dense columns. If columns (in the presolved and aggregated problem) exist with more entries than the value of this option, these columns will be considered "dense" and CPLEX Barrier will treat the dense columns specially in order to reduce their effect. At the default setting of 0, this option is determined automatically, considering factors such as the size of the problem. If a number greater than 0 is entered, this number will be used as the "cutoff" number of entries for considering columns to be dense.



**Note** 

*	If the problem (after Presolve and Aggregator) contains less than 400 rows, dense column handling will not be initiated, regardless of setting of this option.



