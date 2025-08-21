.. _option-CONOPT-penalty_constraints_ratio:


Penalty Constraints Ratio
=========================



:Type:	Floating point number	
:Range:	[0,1]
:Default:	0.1	



This option sets a limit on the ratio of penalty constraints for the No-Penalty Model to be solved. The No-Penalty Model can only be generated and solved if the number of penalty and minimax constraints exceed **Penalty Constraints Ratio**  times the constraints in the Full Model. The default value of this option is 0.1, i.e. the No-Penalty Model is only defined and solved if it is at least 10% smaller than the Full Model.



**Note** 

*	The No-Penalty Model and the Full Model are described in the section :ref:`option-CONOPT-description_of_conopt_algorithm` .




**Learn more about** 

*	:ref:`CONOPT_Description_of_CONOPT_Algorithm` 
*	:ref:`option-CONOPT-use_no-penalty_model`  



