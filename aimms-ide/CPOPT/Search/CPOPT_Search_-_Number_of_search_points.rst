.. _CPOPT_Search_-_Number_of_search_points:


Number of search points
=======================



**Type** :	Integer	

**Range** :	{2..2100000000}	

**Default** :	30	



This option controls the number of (possibly partial) solutions manipulated by the multi-point search algorithm (option **Search Type**  equal to 'Multi point'). The default value is 30. A larger value will diversify the search, with possible improvement in solution quality at the expense of a longer run time. A smaller value will intensify the search, resulting in faster convergence at the expense of solution quality. Note that memory consumption increases proportionally to this parameter, for each search point must store each decision variable domain.



**Learn more about** 

*	:ref:`CPOPT_Search_-_Search_type` 
