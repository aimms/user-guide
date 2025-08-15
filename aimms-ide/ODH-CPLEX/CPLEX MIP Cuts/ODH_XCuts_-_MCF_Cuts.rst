.. _ODH-CPLEX_XCuts_-_MCF_Cuts:


MCF Cuts
========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option determines whether or not to generate multi-commodity flow cuts in a problem where CPLEX detects the characteristics of a multi-commodity flow network with arc capacities. By default, CPLEX decides whether or not to generate such cuts. Possible values are:



*	Off
*	Automatic
*	Generate cuts moderately
*	Generate cuts aggressively




CPLEX is able to recognize the structure of a network as represented in many real-world models. When it recognizes such a network structure, CPLEX is able to generate cutting planes that usually help solve such problems. In this case, the cuts that CPLEX generates state that the capacities installed on arcs pointing into a component of the network must be at least as large as the total flow demand of the component that cannot be satisfied by flow sources within the component.

