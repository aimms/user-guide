.. _CPOPT_Logging_-_Warning_level:


Warning level
=============



**Type**:	Integer	

**Range**:	{0..3}	

**Default**:	2	



This option controls the level of warnings issued by CP Optimizer when a solve is launched. Specifically, all warnings of level higher than this option are masked. Setting this option to 0 turns off all warnings. Warnings issued may indicate potential errors or inefficiencies in your model. The default value of this option is 2.



The warnings (if any) are printed to the status file which is named 'CP Optimizer 22.1.sta' and placed in the log folder.

