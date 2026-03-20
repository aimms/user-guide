

.. _option-Baron-keep_summary_file:


Keep summary file
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether the summary file should be kept after the model is solved. Possible values are:



    *	Off
    *	On




**Note** 

*	The summary file, if any, will be placed in the 'log' directory of the project directory. Its name is determined by the option **File Name**, and its extension is '_sum.lst'.
*	The general solvers option **Progress Time Interval**  influences the amount of logging to the summary file. If it is set to 0 or to a large value then logging is done less frequent.




**Learn more about** 

*	:doc:`BARON_Logging_-_File_name` 
*	:doc:`../../../Aimms/Options/AIMMS/Progress, Errors & Warnings/Progress Options/Progress_Options_-_Progress_Time_Interval` 



