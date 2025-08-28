.. _option-KNITRO-number_of_mip_threads:


Number of MIP Threads
=====================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0		



This option specifies the number of threads to use for MIP branch and bound. The value of 0 lets Knitro choose the number of threads.



This option is effective when the option **MIP Method**  is set to 'Branch_and_bound'.



**Learn more about** 

*	:ref:`option-KNITRO-mip_method`  
