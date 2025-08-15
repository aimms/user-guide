.. _CBC_MIP_Cuts_-_Lift_and_Project_Cuts:


Lift and project cuts
=====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



The value of this option determines if there should be any attempt to generate lift-and-project cuts for the problem. These cuts may be expensive to compute.



Setting the value different from "Off" indicates that the attempt to generate lift-and-project cuts should be made. Setting 'On' means that this cut generator will be tried in the branch-and-cut tree (you can fine tune using option **Cut Depth** ). Setting 'Root only' means just at the root node while 'If promising' means that cuts will be used in the tree if they look as if they are doing some good and moving the objective value. Possible values are:



*	Off
*	On
*	Root only
*	If promising
*	Always




This option is not influenced by the option **Global Cut Control** .





**Learn more about** 

*	:ref:`CBC_MIP_Cuts_-_Cut_Depth`  
*	:ref:`CBC_MIP_Cuts_-_Global_Cut_Control`  
