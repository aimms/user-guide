.. _option-CPLEX-write_parameter_file:


Write Parameter File
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes' a CPLEX parameter file will be written. The file will be named cpxddddd.prm,
where ddddd denotes a 5-digit sequence number. Parameter files are written only if one of the options
**LP File**, **MPS** or **Sav File** is set to 'At the first solve' (in which case a parameter file is written for
the first solve) or 'At every solve' (in which case parameter files for every solve are written).

Possible values of this option are:

    *	No
    *	Yes


A CPLEX parameter (PRM) file is used to specify parameter settings. The file consists of parameter-value pairs, each
on its own line. The following is a simple example:

.. code-block:: text

   CPLEX Parameter File Version 22.1
   CPX_PARAM_PERIND     1
   CPX_PARAM_EPPER      3.45000000000000e-06
   CPX_PARAM_STARTALG   2


The parameters are printed using the CPLEX C API names as can be found in the :ref:`CPLEX_to_AIMMS_Mapping` from AIMMS option
names to CPLEX parameter names.


**Note** 

*	Only parameters (options) with non-default values according to CPLEX will be printed.


**Learn more about** 

*	:ref:`option-CPLEX-lp_file`  
*	:ref:`option-CPLEX-mps`  
*	:ref:`option-CPLEX-sav_file`  
