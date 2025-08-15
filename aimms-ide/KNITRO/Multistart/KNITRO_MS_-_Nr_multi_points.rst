.. _KNITRO_MS_-_Nr_multi_points:


Number of Multistart Points
===========================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



This option specifies how many start points Knitro should try when multistart is used. This option has only effect if the option **Multistart**  is switched on.



The value of 0 has a special meaning; it lets Knitro automatically choose a value based on the problem size. The value is min(200, 10N), where N is the number of variables in the problem.



**Learn more about** 

*	:ref:`KNITRO_MS_-_Multistart`  



