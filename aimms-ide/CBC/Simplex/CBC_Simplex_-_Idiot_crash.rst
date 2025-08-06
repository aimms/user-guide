.. _CBC_Simplex_-_Idiot_crash:


Idiot crash
===========



**Type** :	Integer	

**Range** :	{-1 .. 999999}	

**Default** :	-1	



Idiot crash is a type of 'crash' which works well on some homogeneous problems. It works best on problems with unit elements and right-hand-side but will do something to any model. It should only be used before primal. It can be set to -1 in which case CBC decides whether to use it. A value of 0 switches it off, and for n > 0 it will do n passes.



**Learn more about** 

*	:ref:`CBC_Simplex_-_Crash`  
