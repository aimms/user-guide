.. _option-GUROBI-tune_metric:


Tune Metric
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



A single tuning run typically produces multiple timing results for each candidate option set, either as a result of performing multiple trials, or tuning multiple models, or both. This option controls how these results are aggregated into a single measure. Possible values are:



    *	Automatic
    *	Average
    *	Maximum




The default setting chooses the aggregation automatically; setting 'Average' computes the average of all individual results; setting 'Maximum' takes the maximum.





**Learn more about** 

*	:ref:`GUROBI_Tuning_Tool` 
