.. _option-GUROBI-barrier_progress_solution:


Barrier Progress Solution
=========================



:Type:	Integer	
:Range:	{0 .. 2000000000}	
:Default:	0	



This option controls the progress reports during the solution process if the barrier solver is used by Gurobi. If the
:ref:`aimmshelp12-progress_window` is open, it will display information about the number of (barrier) iterations, the
current status, the best value found, etc. Possible values are: 

.. list-table::
   :width: 60 %
   :widths: 10 90
   :header-rows: 0

   * - 0
     - Do not report progress
   * - *n*
     - Report progress after each *n* barrier iterations


**Note** 

*	This option overrules the setting of the general solvers option **Progress Solution** in case the barrier solver is used, and Gurobi is not in the Barrier crossover phase.


**Learn more about** 

*	:ref:`option-AIMMS-progress_solution` 
