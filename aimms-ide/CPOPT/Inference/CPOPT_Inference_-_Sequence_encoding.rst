.. _CPOPT_Inference_-_Sequence_encoding:


Sequence encoding
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Direct	



This option determines the encoding used for CP::Sequence constraints. Possible values are:



*	Direct
*	Count
*	Partial sum




With setting 'Direct' the AIMMS-CP Optimizer interface uses the IloSequence class of CP Optimizer.





Encoding 'Count' uses IloCount functions of CP Optimizer to write the CP::Sequence constraints explicitly.





Encoding 'Partial sum' follows the encoding proposed by Sebastian Brand, Nina Narodytska, Claude-Guy Quimper, Peter Stuckey and Toby Walsh in Encodings of the SEQUENCE constraint, In: CP. Volume 4741 of LNCS, 2007, pp 210--224, Springer.





**Note** 

*	Encoding 'Direct' is not supported for cyclic CP::Sequence constraints. For cyclic CP::Sequence constraints the 'Count' encoding is used if the setting of this option equals 'Direct'.
*	The mod file is not printed if the value of this option equals 'Direct' or 'Partial sum'.




**Learn more about** 

*	:ref:`CPOPT_Logging_-_Mod_file` 
