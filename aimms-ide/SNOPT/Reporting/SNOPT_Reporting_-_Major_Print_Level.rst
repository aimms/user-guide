.. _SNOPT_Reporting_-_Major_Print_Level:


Major Print Level
=================



**Type**:	Integer	

**Range**:	{0..63}	

**Default**:	1	



This option controls the amount of output that is printed in the output file for each major iteration. This option has only an effect if the option **Print Output File**  is switched on. The value of this option is written as a binary number containing six bits. The bits represent the information printed in the following sense:




.. list-table::

   * - **Bit** 
     - **Value** 
     - **Information** 
   * - 1
     - 1
     - Summary of each major iteration
   * - 2
     - 2
     - Related to basis matrix
   * - 3
     - 4
     - The nonlinear variables
   * - 4
     - 8
     - The dual variables for the nonlinear constraints
   * - 5
     - 16
     - The values of the nonlinear constraint functions
   * - 6
     - 32
     - The Jacobian matrix




For example, to activate 'Summary of each major iteration', 'The nonlinear variables' and 'The Jacobian matrix', set the value of this option to 1+4+32=37. The default value of 1 corresponds to only bit 1 being set.



**Learn more about** 

*	:ref:`SNOPT_Reporting_-_Minor_Print_Level`  
*	:ref:`SNOPT_Reporting_-_Print_Output_File`  
