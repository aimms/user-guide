.. _option-CONOPT-box_size_tolerance_linear:

Box Size Tolerance Linear
=========================



:Type:	Floating point number	
:Range:	[0.01,1e8]
:Default:	1000	



This option specifies the initial box size for trust region models for the Linear Feasibility Model. It is similar to the option **Box Size Tolerance**  but applied to the Linear Feasibility Model. Since this model has linear constraints the default initial box size is larger.



**Note** 

*	More on the Linear Feasibility Model and Phase 0 can be found in the section :ref:`CONOPTDescription_of_CONOPT_Algorithm`.




**Learn more about** 

*	:ref:`option-CONOPT-box_size_tolerance` 
*	:ref:`CONOPT_Description_of_CONOPT_Algorithm` 



