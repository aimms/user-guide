.. _option-CONOPT-box_size_factor_linear_variables:


Box Size Factor Linear Variables
================================



:Type:	Floating point number	
:Range:	[1,1000]
:Default:	10	



This option specifies the box size factor for linear variables applied to trust region box size. The trust region box used in the new Phase 0 method limits the change of variables so 2nd order terms will not become too large. Variables that appear linearly do not have 2nd order terms and the initial box size is therefore larger by a factor equal to the value of this option.



**Note** 

*	More about Phase 0 can be found in the section :ref:`CONOPT_Description_of_CONOPT_Algorithm`.




**Learn more about** 

*	:ref:`CONOPT_Description_of_CONOPT_Algorithm` 



