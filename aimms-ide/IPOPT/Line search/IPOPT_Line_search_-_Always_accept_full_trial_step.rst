

.. _option-IPOPT-always_accept_full_trial_step:


Always accept full trial step
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option specifies whether the first trial step should always be accepted. Setting this option to 'Yes' essentially disables the line search and makes the algorithm take aggressive steps, without global convergence guarantees. Possible values are:



    *	No
    *	Yes



