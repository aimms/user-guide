.. _XA_General_-_Presolve_Activity_Types:


Presolve Activity Types
=======================



:Type:	Integer	
:Range:	{0..8191}	
:Default:	2047	



This option determines which types of model reduction the presolver of XA should perform. This option has only an effect if the setting of the option **Presolve**  is "Yes". To communicate the type of model reduction to XA, the value of this option is written as a binary number containing thirteen bits. The bits represent the model reduction types in the following sense:




.. list-table::

   * - **Bit** 
     - **Value** 
     - **Type of scaling** 
   * - 0
     - 1
     - Singleton column reduction
   * - 1
     - 2
     - Singleton row reduction
   * - 2
     - 4
     - Min/Max row adjust
   * - 3
     - 8
     - Dual checking
   * - 4
     - 16
     - Primal bounds adjust
   * - 5
     - 32
     - Cheap Dual Check
   * - 6
     - 64
     - Identical column
   * - 7
     - 128
     - Dependent rows
   * - 8
     - 256
     - Row doubleton reduction
   * - 9
     - 512
     - Free column reduction
   * - 10
     - 1024
     - Matrix reduction
   * - 11
     - 2048
     - Restore original bounds
   * - 12
     - 4096
     - Expensive dual test




For example, to activate 'Singleton row reduction', 'Dependent rows', 'Free column reduction' and 'Matrix reduction' only, set the value of this option to 2+128+512+1024=1666. The default value of 2047 corresponds to everything activated except 'Restore original bounds' and 'Expensive dual test'.



When you know that your model does not have a lot of unnecessary rows or columns, or if you plan to solve variations of the same model many times, you should consider reducing the amount of presolve checking because these routines can cost a lot of time.



**Learn more about** 

*	:ref:`XA_General_-_Presolve`  



