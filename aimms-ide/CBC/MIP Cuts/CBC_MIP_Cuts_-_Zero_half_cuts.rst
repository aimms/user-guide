.. _option-CBC-zero_half_cuts:


Zero half cuts
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	If promising	



The value of this option determines if there should be any attempt to generate two phase zero-half cuts for the problem. Setting the value different from "Off" indicates that the attempt to generate zero-half cuts should be made. Setting 'On' means that this cut generator will be tried in the branch-and-cut tree (you can fine tune using option **Cut Depth** ). Setting 'Root only' means just at the root node while 'If promising' means that cuts will be used in the tree if they look as if they are doing some good and moving the objective value. Possible values are:



*	Off
*	On
*	Root only
*	If promising
*	Always




This option overrides the option **Global Cut Control** .





So far, zero-half cuts may help only on a small subset of problems and may need some tuning.





**Learn more about** 

*	:ref:`option-CBC-cut_depth`  
*	:ref:`option-CBC-global_cut_control`  




**References** 

*	Andreello, G., A. Caprara and M. Fischetti, Embedding cuts in a branch and cut framework: a computational study with {0,1/2} cuts, INFORMS Journal on Computing **19**  (2007), pp. 229-238.
