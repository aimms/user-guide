

.. _Options_Backward_Compatibility_-_Deriv:


Derive Definitions Stochastic Parameters
========================================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	



Consider the following situation: A parameter P has both a definition and the stochastic property set. The definition of P references parameter Q and parameter Q also has the property stochastic set. When this option is set to 'Off', the parameter P.stochastic does not have a definition. When this option is set to 'On', AIMMS copies the definition of P to P.stochastic, but the definition of P.Stochastic will reference Q.Stochastic instead of just Q. Possible values are:



*	On
*	Off




**Learn more about** 

*	:ref:`sec:stoch.solve`  






