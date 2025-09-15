.. _option-GUROBI-mps_dual:


MPS Dual
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



This option can be used to generate a model file with the dual formulation of the loaded LP model. The model file can be in MPS or LP format.
The generated files are named gur*ddddd*.dua or gur*ddddd*.dlp, where *ddddd* denotes a 5 digits sequence number. Possible values are:

    *	Never
    *	At the first solve (MPS format)
    *	At every solve (MPS format)
    *	At the first solve (LP format)
    *	At every solve (LP format)


**Note** 

*	This option is only supported for LP problems.


**Learn more about** 

*	:ref:`option-GUROBI-mps` 
