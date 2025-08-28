.. _option-ODHCPLEX-sifting_from_simplex:


Sifting from Simplex
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option can be used to turn on (or off) sifting from simplex optimization. By default, sifting from simplex optimization is on. That is, under appropriate conditions, CPLEX invokes sifting from simplex. If you want to force sifting, set the option **MIP Method**  or **MIP Start Algorithm**  to 'Sifting'. Possible values are:



    *	No
    *	Yes




**Learn more about** 

*	:ref:`option-ODHCPLEX-mip_method`  
*	:ref:`option-ODHCPLEX-mip_start_algorithm`  
