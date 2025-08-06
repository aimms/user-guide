.. _CBC_MIP_-_Strong_branching:


Strong branching
================



**Type** :	Integer	

**Range** :	{0 .. 999999}	

**Default** :	5	



This option sets the number of variables to look at in strong branching. In order to decide which variable to branch on, CBC will choose up to this number of unsatisfied variables and try mini up and down branches. The most effective one is chosen. If a variable is branched on many times then the previous average up and down costs may be used.



**Learn more about** 

*	:ref:`CBC_MIP_-_Trust_pseudo_costs` 
