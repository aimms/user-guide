.. _CPOPT_Logging_-_Log_period:


Log period
==========



**Type** :	Integer	

**Range** :	{1..2100000000}	

**Default** :	1000	



The CP Optimizer search log includes information that is displayed periodically. This option controls how often that information is displayed. By setting this parameter to a value of k, the log is displayed every k branches (search decisions).



**Note** 

*	This option is ignored if the option **Log Verbosity**  is set to 'Quiet' or 'Terse'.




**Learn more about** 

*	:ref:`CPOPT_Logging_-_Log_verbosity` 
