

.. _option-AIMMS-initial_column_reservation:


Initial Column Reservation
==========================



:Type:	Integer	
:Range:	{0..10485760}	
:Default:	0	



This option determines the number of variables, corresponding to which memory is reserved to store the model. When solving a sequence of models with a differing number of variables, setting this option to the maximal number of variables is effective, because AIMMS does not have to reallocate memory.



