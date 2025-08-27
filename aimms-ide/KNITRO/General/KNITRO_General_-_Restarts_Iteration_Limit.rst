.. _option-KNITRO-restarts_iteration_limit:


Restarts Iteration Limit
========================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



When **Restarts**  are enabled, this option can be used to specify a maximum number of iterations before enforcing a restart. Possible values are: 



0:	No iteration limit on restarts enforced.

n:	At most n iterations are allowed without convergence before enforcing an automatic restart, if restarts are enabled..



    **Learn more about** 

*	:ref:`option-KNITRO-restarts` 
