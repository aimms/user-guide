

.. _option-IPOPT-nlp_scaling_method:


NLP scaling method
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Gradient based	



This option selects the technique used for scaling the problem internally before it is solved. Possible values are:



    *	None
    *	Gradient based
    *	Equilibration based




Setting 'Gradient based' (the default) means: scale the problem so the maximum gradient at the starting point equals the value of option **Maximum Gradient after NLP Scaling** .





Setting 'Equilibration based' means: scale the problem so that first derivatives are of order 1 at random points (only available with MC19).





**Learn more about** 

*	:ref:`option-IPOPT-maximum_gradient_after_nlp_scaling` 
