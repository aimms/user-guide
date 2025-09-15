.. _option-GUROBI-node_file_start:


Node File Start
===============



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100	



This option controls the point at which MIP tree nodes are written to disk. Whenever node storage exceeds the specified value (in GBytes),
nodes are written to disk.

The node file is written to a subdirectory grbnodes\ *x*\ , with *x* being a nonnegative integer, of the AIMMS project directory.

