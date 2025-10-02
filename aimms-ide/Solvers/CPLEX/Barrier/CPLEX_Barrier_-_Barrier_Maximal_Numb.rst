.. _option-CPLEX-barrier_maximal_number_of_corrections:


Barrier Maximal Number of Corrections
=====================================



:Type:	Integer	
:Range:	{-1 .. 2147483647}	
:Default:	-1	



This option is used to set the maximum number of centering corrections done on each iteration. By default,
the Barrier Solver automatically computes an estimate value for this option (the computed value can be
observed in the CPLEX log by setting the option **Barrier Display** to 'Diagnostics'). When using the default
barrier algorithm, if the computed value is 0, setting the value to an explicit value greater than 0 may
improve the numerical performance of the algorithm at the expense of computation time. Possible values are:

.. list-table::
  :width: 60 %
  :widths: 20 80

   * - -1
     - Automatically determined
   * - 0
     - No corrections
   * - *n*
     - *n* corrections


**Learn more about** 

*	:ref:`option-CPLEX-barrier_display` 

