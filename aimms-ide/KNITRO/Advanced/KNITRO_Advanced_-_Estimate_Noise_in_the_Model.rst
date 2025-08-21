.. _option-KNITRO-estimate_noise_in_the_model:


Estimate Noise in the Model
===========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to enable an estimate of the noise in the model when using finite-difference gradients. Possible values are:



*	No
*	Yes
*	Yes with curvature factor




This noise estimate can then be used to set a finite-difference steplength appropriate for the estimated noise level. This can improve performance on models with noise (e.g. noisy black-box optimization models). The cost of the noise estimation procedure is usually a few extra function evaluations.




