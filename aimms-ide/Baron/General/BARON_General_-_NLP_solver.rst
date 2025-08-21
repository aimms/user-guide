

.. _option-Baron-nlp_solver:


NLP solver
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies the NLP solver to be used. Possible values are:



*	Automatic
*	MINOS
*	SNOPT
*	CONOPT
*	IPOPT
*	FilterSD
*	FilterSQP
*	Standard solvers
*	None




By default, BARON will select the NLP solver and may switch between different NLP solvers during the search, 
based on problem characteristics and solver performance.
Any combination of licensed NLP solvers may be used in that case. 
The solvers IPOPT, FilterSD and FilterSQP will always be available. 
For example, if your AIMMS license allows CONOPT then with the setting 'Automatic' BARON will use CONOPT, 
IPOPT, FilterSD and FilterSQP.





At the setting 'Standard solvers' BARON will use IPOPT, FilterSD and FilterSQP.





A single specific NLP solver can be specified by setting this option to a value other than the default or 'Standard solvers'.





If this option is set to 'None' then BARON will not do any local searches for finding feasible solutions. In general BARON will be less effective without using an NLP solver.





**Note** 

*	Setting the value of this option equal to 'None' is the same as setting the options **Number of Preprocessing Searches**  and **Upper Bounding**  to 0.
*	AIMMS will generate an execution error if an NLP solver is selected that is not allowed by the AIMMS license.




**Learn more about** 

*	:ref:`option-Baron-number_of_preprocessing_searches` 
*	:ref:`option-Baron-upper_bounding` 
*	`FilterSD <https://github.com/coin-or/Ipopt>`_ (Internet link)
*	`IPOPT <https://github.com/coin-or/Ipopt>`_ (Internet link)






