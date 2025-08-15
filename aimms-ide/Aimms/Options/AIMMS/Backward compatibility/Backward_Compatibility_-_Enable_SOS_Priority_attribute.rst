

.. _Options_Backward_Compatibility_-_Enable_SOS_Priority_attribute:


Enable SOS Priority attribute
=============================



**Type**:	Selection	

**Range**:	One of the settings listed below	

**Default**:	Off	



The information from the SOS Priority attribute is only used by CPLEX 9.1 and older. Filling in this attribute may therefore erroneously make a model developer to believe this is a tool to steer the solution process. In order to avoid such confusion, the SOS Priority attribute is by default no longer shown nor saved. This option determines whether or not the SOS Priority attribute is available to constraints with a SOS property. Possible values are:



*	On
*	Off



