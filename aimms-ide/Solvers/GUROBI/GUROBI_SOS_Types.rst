.. _GUROBI_SOS_Types:


SOS Types
=========

Special Ordered Sets (SOSs) are an additional way to specify integrality conditions in a model. They can be one of two types:

*	SOS Type 1. A set of variables (all integer, all continuous, or integer and continuous) for which at most one variable may be non-zero.
*	SOS Type 2. A set of integer or continuous variables for which at most two variables may be non-zero. If two variables are non-zero, they must be adjacent in the set.


Special branching strategies are used within Gurobi to take advantage of SOSs. Gurobi can use different ways to reformulate SOS constraints,
as controlled by the options **SOS1 Encoding** and **SOS2 Encoding**.


**Note** 

*	In case of SOS 1, if there is no ordered relationship among the variables (such that weights cannot be specified or would not be meaningful), other formulations should be used instead of a special ordered set.


**Learn more about** 

*	:ref:`option-GUROBI-sos1_encoding` 
*	:ref:`option-GUROBI-sos2_encoding` 
