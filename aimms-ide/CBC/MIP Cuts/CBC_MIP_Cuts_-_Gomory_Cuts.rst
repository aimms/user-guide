.. _option-CBC-gomory_cuts:


Gomory cuts
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	If promising	



The value of this option determines if there should be any attempt to generate Gomory cuts for the problem. The original cuts - beware of imitations! Having gone out of favor, they are now more fashionable as LP solvers are more robust and they interact well with other cuts. They will almost always give cuts (although in CBC they are limited as to number of variables in cut).



Setting the value different from "Off" indicates that the attempt to generate Gomory cuts should be made. Setting 'On' means that cuts will be tried in the branch-and-cut tree (you can fine tune using option **Cut Depth** ). Setting 'Root only' means just at the root node while 'If promising' means that cuts will be used in the tree if they look as if they are doing some good and moving the objective value. Possible values are:



*	Off
*	On
*	Root only
*	If promising
*	Often
*	Always




This option overrides the option **Global Cut Control** .





**Learn more about** 

*	:ref:`option-CBC-cut_depth`  
*	:ref:`option-CBC-global_cut_control`  
