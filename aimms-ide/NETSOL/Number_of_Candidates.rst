

.. _Number_of_Candidates:
.. _NETSOL_Number_of_Candidates:


Number of Candidates
====================



**Type** :	Integer

**Range** :	{1.. :ref:`Miscellaneous_Maxint`  }	

**Default** :	20



While searching for an entering arc, the number of non-basic arcs that are candidates to enter the basis is limited. The candidate list is limited to the value of this option arcs. In every iteration the reduced cost for each arc on the candidate list is computed, and the one with the most favorable reduced cost is selected to enter the basis. When there are no arcs left that can enter the basis, the candidate list is refilled.

