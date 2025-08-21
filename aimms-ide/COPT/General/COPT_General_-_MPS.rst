.. _option-COPT-mps:


MPS
===



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



This option can be used to generate a model file of the loaded model. The model file can be in MPS or LP format. The generated files are named coptddddd.mps, coptddddd.lp or coptddddd.bin, where ddddd denotes a 5 digits sequence number. Possible values are:



*	Never
*	At the first solve (MPS format)
*	At every solve (MPS format)
*	At the first solve (LP format)
*	At every solve (LP format)
*	At the first solve (BIN format)
*	At every solve (BIN format)



