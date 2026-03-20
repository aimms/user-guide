.. _option-XA-extra_memory:


Extra Memory
============



:Type:	Integer	
:Range:	{0 .. :doc:`Maxint <../../../Aimms/Miscellaneous/Short Descriptions/Maxint>`}	
:Default:	1048576	



Together with the option **Minimal Memory Size**  , this option influences the size of the workspace allocated by XA, which is determined according to the formula



min(100 * number of nonzeros + the value of this option, **Minimal Memory Size**  ).



**Remark** 

This option is ignored if the option **Solver workspace**  has been set to a value different than zero.



**Learn more about** 

*	:doc:`XA_Memory_-_Minimal_Memory_Size <XA_Memory_-_Minimal_Memory_Size>`  
*	:doc:`Memory_-_Solver_Workspace <../../../Aimms/Options/Solvers General/Memory/Memory_-_Solver_Workspace>`  



