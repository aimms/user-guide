.. _KNITRO_General_-_Mark_as_Convex:


Mark as Convex
==============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option can be used to mark a problem as convex. Possible values are:



*	Automatic
*	Off
*	On




Declare the problem as convex by switching on this option or non-convex by switching off this option. Otherwise, Knitro will try to determine this automatically, but may only be able to do so for simple model forms such as QPs or QCPs. If your model is specified as (or automatically determined to be) convex, this will cause Knitro to apply specializations and tunings that are often beneficial for convex models to speed up the solution.





**Note** 

*	Currently this option is only active for the Interior/Direct algorithm, but may be applied to other algorithms in the future.



