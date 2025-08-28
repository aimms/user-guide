.. _option-GUROBI-barrier_crossover_basis:


Barrier Crossover Basis
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines the initial basis construction strategy for crossover. Possible values are:



    *	Automatic
    *	Fast
    *	Robust




The value 'Fast' chooses an initial basis quickly. A value of 'Robust' can take much longer, but often produces a much more numerically stable start basis.

