

.. _IPOPT_NLP_scaling_-_Maximum_gradient_after_NLP_scaling:


Maximum gradient after NLP scaling
==================================



:Type:	Floating point number	
:Range:	[1e-010,1e+019]	
:Default:	100	



This option sets the gradient scaling cut-off. If the maximum gradient is above this value, then gradient based scaling will be performed. Scaling parameters are calculated to scale the maximum gradient back to this value.



**Note** 

*	This option is only used if the option **NLP Scaling Method**  has been set to 'Gradient based'. 




**Learn more about** 

*	:ref:`IPOPT_NLP_scaling_-_NLP_scaling_method` 
