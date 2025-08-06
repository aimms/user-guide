.. _CPOPT_Search_-_Restart_growth_factor:


Restart growth factor
=====================



**Type** :	Floating point number	

**Range** :	[1,inf)	

**Default** :	1.05	



When the option **Search Type**  is set to 'Restart', a depth-first search is restarted after a certain number of failures. This option controls the increase of this number between restarts. If the last fail limit was equal to f after a restart, for the next run the new fail limit will be f  times the value of this option.



The initial fail limit can be controlled with the option **Restart Failure Limit** . 



**Learn more about** 

*	:ref:`CPOPT_Search_-_Restart_failure_limit` 
*	:ref:`CPOPT_Search_-_Search_type` 
