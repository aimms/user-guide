

.. _Threshold_Fraction:
.. _NETSOL_Threshold_Fraction:


Threshold Fraction
==================



**Type** :	Floating point number

**Range** :	[1e-16,1]	

**Default** :	0.15



This option controls when the arcs on the candidate list are dismissed and when the candidate list is refilled. When the candidate list is filled, a threshold is set equal to the value of this option multiplied by the best reduced cost. If, during the subsequent iterations, the reduced cost of the entering arc drops below this threshold value, the candidate list is refilled. The candidate list is refilled by scanning a fixed number of nodes and selecting, for each of those nodes, the arc with the most favorable reduced cost. An arc is added to the candidate list only when its reduced cost exceeds the threshold level. The threshold value is computed as the value of this option times the best reduced cost found so far.

