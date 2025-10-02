.. _option-CPLEX-crash_ordering:


Crash Ordering
==============



:Type:	Integer	
:Range:	{-1 .. 1}	
:Default:	1	



This option determines how CPLEX orders variables relative to the objective function when selecting an initial basis.
Possible values are:



For **LP primal simplex**:

.. list-table::
   :width: 60 %
   :widths: 20 80
   :header-rows: 0

   * - 0
     - Ignore objective coefficients during crash
   * - -1 or 1
     - Alternate ways of using objective coefficients


For **LP dual simplex**:

.. list-table::
   :width: 60 %
   :widths: 20 80
   :header-rows: 0

   * - 0 or -1
     - Aggressive starting basis
   * - 1
     - Default starting basis


For **QP Primal**:

.. list-table::
   :width: 60 %
   :widths: 20 80
   :header-rows: 0

   * - -1
     - Slack basis
   * - 0
     - Ignore Q terms and use LP solver for crash
   * - 1
     - Ignore objective and use LP solver for crash


For **QP Dual**: 

.. list-table::
   :width: 60 %
   :widths: 20 80
   :header-rows: 0

   * - -1
     - Slack basis
   * - 0 or 1
     - Use Q terms for crash

