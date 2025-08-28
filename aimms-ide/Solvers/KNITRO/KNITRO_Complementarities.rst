.. _KNITRO_Complementarities:

Complementarities
=================

In AIMMS, a complementarity condition is defined as follows for a given variable yk and an associated function gk(x,y). (Here the vector x represents the normal variables, and vector y the complementarity variables.)



If lk = -¥ and uk = ¥ then




.. list-table::

   * - 
     - either
     - yk = lk 
     - and
     - gk(x,y) ≥ 0
   * - 
     - or
     - yk = uk 
     - and
     - gk(x,y) ≤ 0
   * - 
     - or
     - lk < yk  < uk 
     - and
     - gk(x,y) = 0.


If lk = -¥ and uk = ¥ then




.. list-table::

   * - 
     - either
     - yk = 0 
     - and
     - Lk < gk(x,y)  < Uk 
   * - 
     - or
     - yk ≥ 0 
     - and
     - gk(x,y) = Lk
   * - 
     - or
     - yk ≤ 0  
     - and
     - gk(x,y) = Uk.


In any other situation, where exactly two of the constants lk, uk, Lk and Uk are finite, then




.. list-table::

   * - 
     - either
     - yk = lk 
     - and
     - Lk ≤ gk(x,y)  ≤ Uk 
   * - 
     - or
     - yk = uk 
     - and
     - Lk ≤ gk(x,y)  ≤ Uk 
   * - 
     - or
     - lk < yk  < uk 
     - and
     - gk(x,y) = Lk
   * - 
     - or
     - lk < yk  < uk 
     - and
     - gk(x,y) = Uk.




**Transformation** 

Knitro uses a different definition. In Knitro, a complementarity condition is a condition which enforces that two variables are

complementary to each other, i.e., the variables y1 and y2 are complementary if the following conditions hold:



	y1 × y2 = 0,  y1 ≥ 0,  y2 ≥ 0.



A complementarity condition modeled in AIMMS is automatically transformed into this formulation by adding slack variables and extra constraints.





