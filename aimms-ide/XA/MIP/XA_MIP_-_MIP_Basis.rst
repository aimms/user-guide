.. _option-XA-mip_basis:


MIP Basis
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines whether the AIMMS basis is loaded or not. If AIMMS provides a basis to XA that is loaded, then no presolving and crashing will be performed. In case of a MIP model this may lead to a loss of performance and it may be better to refrain from loading the basis. Possible values are:



    *	No
    *	Yes



