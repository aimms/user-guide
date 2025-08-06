.. _CPOPT_Search_-_Dynamic_probing_strength:


Dynamic probing strength
========================



**Type** :	Floating point number	

**Range** :	[0.001,10000]	

**Default** :	0.03	



This option controls the effort which is dedicated to dynamic probing. It is expressed as a factor of the total search effort: changing this parameter has no effect unless the option **Dynamic Probing**  is set to 'Automatic' or 'On'. When option Dynamic Probing has value 'On', the probing strength is held constant throughout the search process. When option Dynamic Probing has value 'Automatic', the probing strength starts off at the specified value and is thereafter adjusted automatically.



Possible values for this parameter range from 0.001 to 10000. A value of 1.0 indicates that dynamic probing will consume a roughly equal amount of effort as the rest of the search. The default value of this parameter is 0.03, meaning that around 3% of total search time is dedicated to dynamic probing.



**Learn more about** 

*	:ref:`CPOPT_Search_-_Dynamic_probing` 
