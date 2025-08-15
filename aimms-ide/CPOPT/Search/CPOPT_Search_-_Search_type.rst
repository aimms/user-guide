.. _CPOPT_Search_-_Search_**Type**:


Search type
===========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic



This parameter determines the type of search that is applied when solving a problem. When set to 'Depth first' a regular depth-first search is applied. When set to 'Restart' a depth-first search that restarts from time to time is applied. When set to 'Multi point' a method that combines a set of - possibly partial - solutions is applied.



Possible values are:



*	Automatic
*	Depth first
*	Restart
*	Multi point
*	Iterative diving
*	Neighborhood




Iterative diving is a search method that attempts to quickly build feasible solutions and improve them using consecutive iterations of backtrack-free search. It is particularly useful for large (scheduling) problems involving activities. This search method is not available for all problems (in particular it works only on problems with activities). When specified on a problem where iterative diving cannot be applied, the ‘Automatic’ search is used instead.





When the search type is set to 'Automatic' in sequential mode (i.e., option **Number of Workers**  equals 1), restart search will be used in general. In parallel mode, when search type is set to 'Automatic', different searches among restart and multi-point are automatically dispatched over the workers; otherwise all the workers execute the type of search specified by search type.





The default search strategy is different when at least four workers are used. Namely, when scheduling problems (ones with at least one activity) are solved, every fourth worker behaves in a different manner, using a more aggressive diving technique to find solutions to large problems more quickly. Should you find that this degrades performance on your model, you can set this option to 'Restart'.





The value 'Neighborhood' is new in CP Optimizer If this value is selected then a local search method will be used on all workers. The local search method works on full assignments and so can explore assignments which violate constraints. By changing small parts of the current assignment, the search method tries to reduce the constraint violation. If the search finds a feasible solution (zero violations), the search will then also work on optimizing the objective. The search works best on lightly constrained problems. This feature is experimental, and will remain in Beta in CP Optimizer. Feedback is welcome at cos-beta@wwpdl.vnet.ibm.com.





**Note** 

*	Starting point information is used by the restart and multi-point search types only. It is not used by the depth-first search.
*	Neighborhood search cannot be used for scheduling problems (with at least one activity).




**Learn more about** 

*	:ref:`CPOPT_Search_-_Dynamic_probing` 
*	:ref:`CPOPT_Search_-_Number_of_search_points` 
*	:ref:`CPOPT_Parallel_-_Number_of_workers` 
*	:ref:`CPOPT_Search_-_Restart_failure_limit` 
*	:ref:`CPOPT_Search_-_Restart_growth_factor` 
*	:ref:`CPOPT_General_-_Starting_point` 



