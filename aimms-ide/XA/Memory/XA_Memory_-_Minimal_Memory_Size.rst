.. _XA_Memory_-_Minimal_Memory_Size:


Minimal Memory Size
===================



**Type**:	Integer	

**Range**:	{0..:ref:`Miscellaneous_Maxint`  }	

**Default**:	65536	



Together with the option **Extra Memory** , this option influences the size of the workspace allocated by XA, which is determined according to the formula



max(100 ** number of non-zeros + **Extra Memory**  , the value of this option).



**Learn more about** 

*	:ref:`XA_Memory_-_Extra_Memory`  
*	:ref:`Options_Memory_-_Solver_Workspace`  



