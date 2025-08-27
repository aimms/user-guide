.. _option-CPLEX-barrier_ordering:


Barrier Ordering
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option can be used to set the algorithm to be used to permute the rows of the constraint matrix in order to reduce fill in the Cholesky factor. There are three alternative algorithms: Approximate Minimum Degree (AMD), Approximate Minimum Fill (AMF), and Nested Dissection (ND). The default automatic option will usually be the best choice. This setting attempts to choose the most effective of the available algorithms. It usually requires more ordering runtime than any of the alternatives, but it typically chooses the best ordering. The ordering time is usually small relative to the total solution time, and a better ordering can lead to smaller total solution time.



The AMD algorithm provides good quality ordering in moderate ordering runtime. AMF usually gives better orderings than AMD (5-10% smaller factors), but requires somewhat more runtime (10-20%). ND often produces significantly better ordering than AMD and AMF. However, this option sometimes produces worse orderings, and it requires much more ordering runtime. Possible values are:



    *	Automatic
    *	Approximate minimum degree
    *	Approximate minimum fill
    *	Nested dissection



