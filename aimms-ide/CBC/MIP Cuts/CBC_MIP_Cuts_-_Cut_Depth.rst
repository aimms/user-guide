.. _CBC_MIP_Cuts_-_Cut_Depth:


Cut depth
=========



**Type** :	Integer	

**Range** :	{-1 .. 999999}	

**Default** :	-1	



This option controls the depth in the branch-and-cut tree at which to do cuts. Cut generators may be off, or switched on only at the root, or switched on if they look useful, or switched on at some interval. Cuts are added whenever the depth in the tree is a multiple of k where k is the value of this option. The default value of -1 means "off".

