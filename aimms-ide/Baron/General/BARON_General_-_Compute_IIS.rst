

.. _Baron_General_-_Compute_IIS:


Compute IIS
===========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



In case of an infeasible problem, this option can be used to search for an irreducibly inconsistent system (IIS), in case the general solvers option **Infeasibility Finder**  is switched on. Possible values are:



*	Off
*	Algorithm 1
*	Algorithm 2
*	Algorithm 3
*	Algorithm 4
*	Algorithm 5




Algorithm 1 is based on a fast heuristic that may result in an infeasible set that could be possibly further reduced. Algorithm 2 uses a deletion filtering algorithm. Algorithm 3 uses an addition filtering algorithm. Algorithm 4 uses an addition-deletion filtering algorithm. Algorithm 5 uses a depth-first search algorithm.





The option **IIS Include Integers**  determines whether or not general integer variables should be considered as potential members of an IIS.





**Learn more about** 

*	:ref:`Baron_General_-_IIS_include_integers` 
*	:ref:`Options_Solution_-_Infeasibility_Finde`  
