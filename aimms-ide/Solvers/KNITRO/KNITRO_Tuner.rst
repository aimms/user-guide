.. _KNITRO_Tuner:


Tuner
=====

Knitro offers the Knitro-Tuner to try to help you identify some non-default options settings that may improve performance on a particular model or set of models. There are two ways to use the tuner. The first option, called default tuning, only requires setting one option after which Knitro will automatically try different option settings. With the second option, called custom tuning, you can tell Knitro which options (and option settings) it should try for tuning.



**Default Tuning** 

If you are unsure about what Knitro options should be tuned to try to improve performance when running Knitro on your model, then you can simply run the default Knitro-Tuner by setting the option **Tuner**  to 'Automated'. This will cause Knitro to automatically run your model with a variety of automatically determined option settings, and report some statistics at the end. Any Knitro options that have been set in the usual way will remain fixed throughout the tuning procedure.



**Custom Tuning** 

If you have some ideas about which Knitro options you want to tune, then you can tell Knitro which options you want it to tune (as well as specify the values for particular options that you want Knitro to explore). This can be

done by specifying a Tuner options file. A Tuner options file is a simple text file in which you can:



*	Define multiple values (separated by spaces) for each option. This tells Knitro the values you want it to explore.
*	Specify an option name without any values. This will tell Knitro to explore all possible option values for that option. This only works for options that have a finite set of possible option value settings.




All possible combinations of options/values specified in a Tuner options file will be explored by Knitro, while any Knitro options that have been set in the usual way will remain fixed throughout the tuning procedure.





**Tuner Options File** 


The Tuner options file is named 'knitro_tuner_file.txt' and should be placed in the directory of the AIMMS project. The option names used are the Knitro names. The Knitro name belonging to an AIMMS option can be found in the :ref:`AIMMS_to_KNITRO_Mapping` from AIMMS option names to Knitro option names.





As an example, consider the following text in the Tuner options file:





algorithm        


bar_directinterval 0 1 10


bar_murule        


pivot 1e-8 1e-14     





This options file tells the Knitro-Tuner to explore all possible option values for the algorithm (AIMMS: :ref:`option-KNITRO-algorithm`) and bar_murule (AIMMS: :ref:`option-KNITRO-initial_barrier_parameter_value`) options, while exploring three values (0, 1 and 10) for the bar_directinterval (AIMMS: :ref:`option-KNITRO-direct_step_interval`) option and two values (1e-8 and 1e-14) for the pivot (AIMMS: :ref:`option-KNITRO-initial_pivot_treshold`) option.





**Tuner Output** 


The Tuner output, by default, provides a summary line of output for each solve during the tuning process indicating the results of that particular solve. When the Tuner completes all solves, it reports the non-default option settings for the fastest solve. Perhaps more insightful, however, is a summary table of statistics provided by the Tuner at the end of the solve. For example, we may see something like this:





``Summary Statistics`` 


``---------------------------------------------------------------------------`` 


``Percent  Average   Average`` 


``Option Name     Value   #Runs  Optimal #FuncEvals   Time`` 


``-------------------- ---------- -------- ------- ---------- ----------`` 


``bar_directinterval      0    24  100.00     9.1    0.000`` 


``bar_directinterval      1    24  100.00     8.0    0.000`` 


``bar_directinterval     10    24  100.00     8.0    0.000`` 


``-------------------- ---------- -------- ------- ---------- ----------`` 


``bar_murule      1    12  100.00     8.0    0.000`` 


``bar_murule      2    12  100.00    10.3    0.000`` 


``bar_murule      3    12  100.00     8.0    0.000`` 


``bar_murule      4    12  100.00     8.3    0.000`` 


``bar_murule      5    12  100.00     8.0    0.000`` 


``bar_murule      6    12  100.00     7.5    0.000`` 


``-------------------- ---------- -------- ------- ---------- ----------`` 


``pivot  1.00e-08    37  100.00     8.4    0.000`` 


``pivot  1.00e-14    37  100.00     8.4    0.000`` 


``-------------------- ---------- -------- ------- ---------- ----------`` 


``algorithm      1    36  100.00    12.7    0.001`` 


``algorithm      2    36  100.00     6.0    0.000`` 


``algorithm      3     2  100.00     5.0    0.002`` 


``algorithm      4     2  100.00     3.0    0.011`` 


``---------------------------------------------------------------------------`` 





This table indicates the option values explored, the number of Tuner runs for each option value, the percentage of those runs where it found an optimal solution, the average number of function evaluations (in the cases where it found an optimal solution), and the average time (in the cases where it found an optimal solution). In this particular example, the model tested is very small, so the solution times are generally near 0.





This summary table provides some global view of which option settings may be preferable. For example, the table above suggests that algorithm = 2 (which corresponds to setting 'Interior-CG' for AIMMS option :ref:`option-KNITRO-algorithm`) may be preferable for models of this type since it (on average) requires fewer function evaluations and less time to find an optimal solution. The table also suggests that perhaps the non-default setting bar_murule = 6 (which corresponds to setting 'Quality' for AIMMS option :ref:`option-KNITRO-initial_barrier_parameter_value`) should be used, since it requires, on average, the fewest number of function evaluations to converge, although other values are only slightly worse.





The Tuner output is written to the file 'knitro.log' if the option **Status File Display**  is set to a non-default value.





**Learn more about** 

*	:ref:`option-KNITRO-status_file_display`  
*	:ref:`option-KNITRO-tuner`  
*	:ref:`AIMMS_to_KNITRO_Mapping`  
