.. _GUROBI_Solution_Pool_-_Pool_Size:


Pool Size
=========



:Type:	Integer	
:Range:	{1 .. 2000000000}	
:Default:	10	



This option determines how many MIP solutions are stored. For non-default values of the option **Pool Search Mode** , this option sets a target for how many solutions to find, so larger values will impact performance.



**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`GUROBI_Solution_Pool_-_Pool_Search_Mode` 
