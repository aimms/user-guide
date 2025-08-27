.. _option-ODHCPLEX-node_cuts:


Node Cuts
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The value of this option decides whether or not cutting planes are separated at the nodes of the branch-and-bound tree. Possible values are:



    *	Off
    *	Automatic
    *	Generate cuts moderately
    *	Generate cuts aggressively
    *	Generate cuts very aggressively




CPLEX typically separates cutting planes both at the root node and at the tree nodes of the branch-and-bound tree. This option allows you to control the effort that CPLEX should spend in separating cutting planes at the tree nodes. In particular, setting the value of this option to 'Off' completely disables the separation of cutting planes in the tree, but it has no impact on the cut separation applied at the root node.




