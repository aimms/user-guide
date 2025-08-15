

.. _Baron_General_-_IIS_include_integers:


IIS include integers
====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



When a search for an irreducibly inconsistent system (IIS) is requested through the option **Compute IIS** , BARON assumes that the model is unlikely to include an error in terms of binaries, i.e., the bounds on binary variables are always enforced and not considered to be part of an IIS. General integer variables may be considered as part of an IIS or not by using this option, which can take the following values:



*	Off
*	On




If this option is switched on then general integer variables should be considered as potential members of an IIS, i.e., bounds on general integer variables are questioned. Integrality is always enforced.





**Learn more about** 

*	:ref:`Baron_General_-_Compute_IIS` 
