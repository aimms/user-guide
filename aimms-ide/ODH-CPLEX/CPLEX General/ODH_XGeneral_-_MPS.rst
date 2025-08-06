.. _ODH-CPLEX_XGeneral_-_MPS:


MPS
===



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Never	



By setting this option different from "Never", a MPS file will be generated which can be used to solve the model using the CPLEX Interactive Optimizer. If a basis and/or SOS are present, they are written to a separate file also. The generated files start with cpx followed by a five-digit number and one of the following extensions:




.. list-table::

   * - .mps
     - MPS file
   * - .bas
     - Basis file
   * - .sos
     - SOS file




Possible values of this option are:



*	Never
*	At the first solve
*	At every solve






