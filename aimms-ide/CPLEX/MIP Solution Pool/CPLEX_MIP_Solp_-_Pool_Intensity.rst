.. _CPLEX_MIP_Solp_-_Pool_Intensity:


Pool Intensity
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls the trade-off between the number of solutions generated for the solution pool and the amount of time or memory consumed. Possible values are:



*	Automatic
*	Mild
*	Moderate
*	Aggressive
*	Very aggressive




The populate algorithm. The values from 'Mild' to 'Very aggressive' invoke increasing effort to find larger numbers of solutions. Higher values are more expensive in terms of time and memory but are likely to yield more solutions.





For the MIP optimization in the first phase, increasing the value of this option corresponds to increasing the amount of effort spent setting up the branch and cut tree to prepare for a subsequent call to the populate algorithm. For the populate algorithm, increasing the value of this option corresponds, in addition, to increasing the amount of effort spent exploring the tree to generate more solutions. Increase the value of this option only if too few solutions are generated.





Its default value 'Automatic' lets CPLEX choose which intensity to apply. For value 'Mild', the performance of the MIP optimization is not affected. There is no slowdown and no additional consumption of memory due to this setting. However, populate will quickly generate only a small number of solutions. Generating more than a few solutions with this setting will be slow. When you are looking for a larger number of solutions, use a higher value of this option.





For value 'Moderate', some information is stored in the branch and cut tree so that it is easier to generate a larger number of solutions. This storage has an impact on memory used but does not lead to a slowdown in the performance of the MIP optimization. With this value, calling populate is likely to yield a number of solutions large enough for most purposes. This value is a good choice for most models.





For value 'Aggressive', the algorithm is more aggressive in computing and storing information in order to generate a large number of solutions. Compared to values 'Mild' and 'Moderate', this value will generate a larger number of solutions, but it will slow the MIP optimization and increase memory consumption. Use this value only if setting this option to 'Moderate' does not generate enough solutions.





For value 'Very aggressive' , the algorithm generates all solutions to your model. Even for small models, the number of possible solutions is likely to be huge; thus enumerating all of them will take time and consume a large quantity of memory.





This option has only meaning if the option **Do Populate**  is switched on.





**Learn more about** 

*	:ref:`CPLEX_MIP_Solp_-_Do_Populate`  



