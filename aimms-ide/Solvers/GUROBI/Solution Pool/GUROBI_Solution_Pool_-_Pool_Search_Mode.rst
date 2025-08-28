.. _option-GUROBI-pool_search_mode:


Pool Search Mode
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Normal	



Gurobi offers different modes for exploring the MIP search tree, as controlled by this option. Possible values are:



    *	Normal
    *	Find additional solutions
    *	Find best solutions




With the default setting ('Normal'), the MIP solver tries to find an optimal solution to the model. By setting this option to a non-default value, the MIP search will continue after the optimal solution has been found in order to find additional, high-quality solutions. With the setting of 'Find best solutions', it will find the n best solutions, where n is determined by the value of the option **Pool Size** . With a setting of 'Find additional solutions', it will try to find additional solutions, but with no guarantees about the quality of those solutions. The cost of the solve will increase with increasing values of this option.





Obtaining an OPTIMAL optimization return status with setting ''Find best solutions' indicates that the MIP solver succeeded in finding the desired number of best solutions, or it proved that the model does not have that many distinct feasible solutions.





**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`option-GUROBI-pool_size` 
