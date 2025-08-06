.. _CBC_MIP_Cuts_-_Global_Cut_Control:


Global cut control
==================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	On	



This option provides a global cut control, affecting the generation of all cuts (except lift-and-project cuts and residual capacity cuts). Setting the value different from "Off" indicates that the attempt to generate cuts should be made. Setting 'On' means that cuts will be tried in the branch-and-cut tree (you can fine tune using option **Cut Depth** ). Setting 'Root only' means just at the root node while 'If promising' means that cuts will be used in the tree if they look as if they are doing some good and moving the objective value. Possible values are:



*	Off
*	On
*	Root only
*	If promising
*	Always




Setting the value of this option to 'Root only' would apply all cut types (except lift-and-project cuts and residual capacity cuts) at the root node of the branch-and-cut tree, unless the cut specific option is set. For example, if the value of this option is set to 'Root only' and the value of option **Clique Cuts**  is set to 'Off' then all cut types will be generated at the root node, except clique cuts which would not be generated at all.





**Learn more about** 

*	:ref:`CBC_MIP_Cuts_-_Clique_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_Flow_Cover_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_Gomory_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_Knapsack_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_Lift_and_Project_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_MIR_Cuts`  
*	:ref:`CBC_MIP_Cuts_-_Probing_cuts`  
*	:ref:`CBC_MIP_Cuts_-_Reduce_and_split_cuts`  
*	:ref:`CBC_MIP_Cuts_-_Residual_capacity_cuts`  
*	:ref:`CBC_MIP_Cuts_-_Two_MIR_cuts`  
*	:ref:`CBC_MIP_Cuts_-_Zero_half_cuts`  
