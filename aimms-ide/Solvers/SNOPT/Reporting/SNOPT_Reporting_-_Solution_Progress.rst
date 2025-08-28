.. _option-SNOPT-solution_progress:


Solution Progress
=================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



This option controls the progress reports during the solution process of SNOPT. If the Progress Window is open, it will display information about the number of iterations, the current status, etc. Possible values are:



0:	Do not report progress.

n:	Report progress after each n iterations.



    **Note** 

*	The global solvers option **Progress Solution**  has no effect on SNOPT.



