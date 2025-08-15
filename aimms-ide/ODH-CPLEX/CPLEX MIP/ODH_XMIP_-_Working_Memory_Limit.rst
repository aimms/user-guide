.. _ODH-CPLEX_XMIP_-_Working_Memory_Limit:


Working Memory Limit
====================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	2048	



This option specifies an upper limit on the amount of central memory, in megabytes, that CPLEX is permitted to use for working memory before compressing memory, swapping to disk files, or taking other actions.



These actions are defined by the option **Node File** , which controls how CPLEX behaves when specifying this limit.



**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_Node_File`  



