.. _option-CBC-reduce_and_split_cuts:


Reduce and split cuts
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off



The value of this option determines if there should be any attempt to generate reduce-and-split cuts for the problem. Setting the value different from "Off" indicates that the attempt to generate reduce-and-split cuts should be made. Setting 'On' means that this cut generator will be tried in the branch-and-cut tree (you can fine tune using option **Cut Depth** ). Setting 'Root only' means just at the root node while 'If promising' means that cuts will be used in the tree if they look as if they are doing some good and moving the objective value. Possible values are:



    *	Off
    *	On
    *	Root only
    *	If promising
    *	Always




This option overrides the option **Global Cut Control**.





**Learn more about** 

*	:ref:`option-CBC-cut_depth`  
*	:ref:`option-CBC-global_cut_control`  
