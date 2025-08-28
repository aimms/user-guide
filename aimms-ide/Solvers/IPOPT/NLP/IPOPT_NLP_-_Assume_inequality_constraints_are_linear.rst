

.. _option-IPOPT-assume_inequality_constraints_are_linear:


Assume inequality constraints are linear
========================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option indicates whether all inequality constraints are linear. Activating this option will cause IPOPT to ask for the Jacobian of the inequality constraints only once for the NLP and reuse this information later. Possible values are:



    *	No
    *	Yes



