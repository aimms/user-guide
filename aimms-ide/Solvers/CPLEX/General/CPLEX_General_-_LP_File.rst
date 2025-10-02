.. _option-CPLEX-lp_file:


LP File
=======



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



This option can be used to generate a CPLEX LP file (or model file) of the current model loaded. The model is written to a
file called cpx\ *ddddd*\ .lp, where *ddddd* denotes a 5 digit sequence number. Possible values are:

    *	Never
    *	At the first solve
    *	At every solve


If the model contains diversity filters or range filters (and the model type is MIP, MIQP or MIQCP), then the filters are written
to a FLT file called cpx\ *ddddd*\ .flt.

