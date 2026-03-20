.. _option-SNOPT-minor_print_level:


Minor Print Level
=================



:Type:	Integer	
:Range:	{0..10}	
:Default:	1	



This option controls the amount of output that is printed to the output file during the solution of the QP subproblems. Its value has the following effect:




.. list-table::

   * - 0
     - No minor iteration output except error messages.
   * - 1-9
     - A single line of output each minor iteration as controlled by the option **Print Frequency**.
   * - 10
     - Basis factorization statistics generated during the periodic refactorization of the basis (see the option **Factorization Frequency**). Statistics for the first factorization for each major iteration are controlled by the option **Major Print Level**.




This option has only an effect if the option **Print Output File**  is switched on. 



**Learn more about** 

*	:doc:`SNOPT_Advanced_-_Factorization_Frequ <../Advanced/SNOPT_Advanced_-_Factorization_Frequ>`  
*	:doc:`SNOPT_Reporting_-_Major_Print_Level <SNOPT_Reporting_-_Major_Print_Level>`  
*	:doc:`SNOPT_Reporting_-_Print_Frequency <SNOPT_Reporting_-_Print_Frequency>`  
*	:doc:`SNOPT_Reporting_-_Print_Output_File <SNOPT_Reporting_-_Print_Output_File>`  
