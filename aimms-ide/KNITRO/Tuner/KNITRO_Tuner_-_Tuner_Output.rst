.. _option-KNITRO-tuner_output:


Tuner Output
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



This option can be used to enable writing output to files for each solve of the Knitro-Tuner procedure. Possible values are:



    *	None
    *	Summary
    *	All




If this option is set to 'Summary' then Knitro will print one line for each solve in the files 'knitro_tuner_summary.log' and 'knitro_tuner_summary.csv' (which is a file that can be opened with Excel).





If this option is set to 'All' then, in addition to creating the summary files, Knitro will print an iteration log for each solve. These files are named 'knitro_tuner_xxx.log', where xxx denotes the sequence number of the solve. This might result in many large files being created. Normally it is sufficient to only print the Tuner output which provides a summary line of output for each solve during the tuning process indicating the results of that particular solve.





This option only has effect if the option **Tuner**  is switched on.





**Note** 

*	The Tuner summary is also written to the file 'knitro.log' if the option **Status File Display**  is set to a non-default value.




**Learn more about** 

*	:ref:`option-KNITRO-status_file_display`  
*	:ref:`option-KNITRO-tuner`  
