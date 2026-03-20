.. _option-XA-minimal_memory_size:


Minimal Memory Size
===================



:Type:	Integer	
:Range:	{0 .. :doc:`../../../Aimms/Miscellaneous/Short Descriptions/Maxint`}	
:Default:	65536	



Together with the option **Extra Memory**, this option influences the size of the workspace allocated by XA, which is determined according to the formula



max(100 ** number of non-zeros + **Extra Memory**  , the value of this option).



**Learn more about** 

*	:doc:`XA_Memory_-_Extra_Memory`  
*	:doc:`../../../Aimms/Options/Solvers General/Memory/Memory_-_Solver_Workspace`  



