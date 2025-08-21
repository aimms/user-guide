.. _option-CONOPT-box_size_tolerance:

Box Size Tolerance
==================



:Type:	Floating point number	
:Range:	[0.01,1e6]
:Default:	10	



This option specifies the initial box size for trust region models for the overall model. The Phase 0 methods solves an LP model based on a scaled and linearized version of the model with an added trust region box constraint around the initial point. This option defines the size of the initial trust region box. During the optimization the trust region box is adjusted based on how well the linear approximation fits the real model.



**Note** 

*	More about Phase 0 can be found in the section :ref:`option-CONOPT-description_of_conopt_algorithm` .




**Learn more about** 

*	:ref:`option-CONOPT-description_of_conopt_algorithm` 



