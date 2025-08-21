.. _option-CPLEX-mip_probing:


MIP Probing
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The setting of this option determines the amount of variable probing performed on the problem. Probing can be both very powerful and very time consuming. Setting this option to "Limited probing", "More probing", or "Full probing" can result in dramatic reductions or dramatic increases in solution time on particular models. Possible values are:



*	No probing
*	Automatic
*	Limited probing
*	More probing
*	Full probing




The probing feature can help in many different ways on difficult models. Probing is a technique that looks at the logical implications of fixing each binary variable to 0 or 1. It is performed after preprocessing and before the solution of the root relaxation. Probing can be expensive, so this option should be used selectively. On models that are in some sense easy, the extra time spent probing may not reduce the overall time enough to be worthwhile. On difficult models, probing may incur very large runtime costs at the beginning and yet pay off with shorter overall runtime. When you are tuning performance, it is usually because the model is difficult, and then probing is worth trying.





**Learn more about** 

*	:ref:`option-CPLEX-probing_time` 
