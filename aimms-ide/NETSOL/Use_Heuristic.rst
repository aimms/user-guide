

.. _Use_Heuristic:
.. _NETSOL_Use_Heuristic:


Use Heuristic
=============



**Type** :	Selection

**Range** :	The settings listed below	

**Default** :	On



This option controls whether or not the heuristic is used to construct an initial basic solution. If the heuristic is not used, the initial basis is constructed using only artificial arcs. Constructing a completely artificial basis is useful for assuring that the initial basis is strongly feasible. If the initial basis is strongly feasible, the algorithm will not cycle. The value 1 indicates that the heuristic will be used. Possible values are:



q Off

q On



