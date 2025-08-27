

.. _option-AIMMS-progress_time_interval:


Progress Time Interval
======================



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	2	



This option controls the progress reports during the solution process based on the number of seconds. If the Progress Window is open, it will display information about the number of iterations, the current status, the best value found, etc. Possible values are:



0:	Do not report progress.	

n:	Report progress after each n seconds.	



The option **Progress Solution**  can be used to control progress reports based on the number of iterations. By default, progress reports are based on elapsed time only.



    **Note** 

*	This option, together with the option**Progress Solution** , also influences the responsiveness of AIMMS during a solve. If both options are set to 0 or a large value then AIMMS will become less responsive.
*	This option also specifies the interval for calling the time callback procedure, if installed.




**Learn more about** 

*	:ref:`option-AIMMS-progress_solution` 
