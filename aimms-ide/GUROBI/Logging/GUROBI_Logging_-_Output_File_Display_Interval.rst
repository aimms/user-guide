.. _option-GUROBI-output_file_display_interval:


Output File Display Interval
============================



:Type: 	Integer
:Range: 	{1 .. 2000000000}
:Default: 	5



This option controls the frequency at which log lines are printed (in seconds) to the Gurobi output file. The option **Output File**  should be set to 'Yes' to generate a Gurobi output file.



**Note** 

*	This option also has an influence on the progress updates, as controlled by the general solvers options **Progress Solution**  and **Progress Time Interval** . If this option is set to a large value then progress updates are done less frequent.




**Learn more about** 

*	:ref:`option-GUROBI-output_file` 
*	:ref:`Options_Progress_Options_-_Progress_Co` 
*	:ref:`Options_Progress_Options_-_Progress_Time_Interval` 
