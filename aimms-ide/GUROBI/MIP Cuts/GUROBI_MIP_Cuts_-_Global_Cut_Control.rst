.. _GUROBI_MIP_Cuts_-_Global_Cut_Control:


Global Cut Control
==================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option provides a global cut control, affecting the generation of all cuts. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive
*	Very aggressive




Setting the value of this option to 'Aggressive' would apply all cut types aggressively, unless the cut specific option is set. For example, if the value of this option is set to 'Aggressive' and the value of option **Clique Cuts**  is set to 'Off' then all cut types will be generated aggressively, except clique cuts which would not be generated at all.





**Learn more about** 

*	:ref:`GUROBI_MIP_Cuts_-_Clique_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Cover_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Dual_Implied_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Flow_Cover_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Flow_Path_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_GUB_Cover_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Implied_Bound_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_MIP_Separation_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_MIR_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Mixing_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Mod_K_cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Network_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Projected_Implied_Bound_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Sub_MIP_Cuts`  
*	:ref:`GUROBI_MIP_Cuts_-_Zero_Half_Cuts`  



