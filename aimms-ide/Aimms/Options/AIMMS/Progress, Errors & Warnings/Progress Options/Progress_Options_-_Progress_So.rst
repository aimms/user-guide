

.. _Options_Progress_Options_-_Progress_So:


Progress Solution
=================



Type:	Integer	

Range:	{0..:ref:`Miscellaneous_Maxint`  }	

Default:	0	



This option controls the progress reports during the solution process based on the number of iterations. If the Progress Window is open, it will display information about the number of iterations, the current status, the best value found, etc. Possible values are:



0:	Do not report progress.	

n:	Report progress after each n iterations.	



The option **Progress Time Interval**  can be used to control progress reports based on the number of seconds. By default, progress reports are based on elapsed time only.



**Note** 

*	This option, together with the option**Progress Time Interval** , also influences the responsiveness of AIMMS during a solve. If both options are set to 0 or a large value then AIMMS will become less responsive.
*	This option is not supported by the following solvers SNOPT, MINOS, PATH, KNITRO, BARON and CP Optimizer. SNOPT, MINOS and PATH each use a solver specific option named **Solution Progress** . Progress updates by BARON, KNITRO and CP Optimizer are only based on elapsed time.




**Learn more about** 

*	:ref:`Options_Progress_Options_-_Progress_Time_Interval` 



