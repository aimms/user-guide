.. _option-CBC-mip_basis:


MIP basis
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By switching on this option the user can pass a basis to CBC for a MIP model that can be used by CBC for solving the first LP in the branch-and-bound tree search. The value of the general solvers option **Accept Basis**  should also be set to such a value that the basis will be accepted; if the value of the option **Accept Basis**  is 0 then AIMMS wil not pass a basis to CBC.



A side effect of passing a basis to CBC is that no presolving. In case of a MIP model this will in general lead to a loss of performance. Possible values are:



    *	No
    *	Yes




**Learn more about** 

*	:ref:`option-AIMMS-accept_basis`  
