.. _CBC_General_-_Sifting:


Sifting
=======



:Type:	Integer	
:Range:	{-1 .. 5000000}	
:Default:	-1	



For long and thin problems CBC may solve a series of small problems created by taking a subset of the columns. The idea was introduced as 'Sprint' after an LP code of that name of the 60's which tried the same tactic (not totally successfully). CPLEX calls it 'sifting'.



At the default value of -1 CBC decides. A value of 0 means that sifting is switched off. For a positive value it specifies the number of passes.

