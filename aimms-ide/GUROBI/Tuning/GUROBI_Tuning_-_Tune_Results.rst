.. _GUROBI_Tuning_-_Tune_Results:


Tune Results
============



:Type:	Integer	
:Range:	{-1 .. 2000000000}	
:Default:	-1



The tuning tool often finds multiple option sets that produce better results than the baseline settings. This option controls how many of these sets should be retained when tuning is complete. The default value of -1 retains the best results that were found for each count of changed options. In other words, it retains the best result for one changed option, for two changed options, etc. Results that aren't on the efficient frontier are discard.



**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`GUROBI_Tuning_Tool` 
