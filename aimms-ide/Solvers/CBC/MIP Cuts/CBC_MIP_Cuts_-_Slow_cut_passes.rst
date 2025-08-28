.. _option-CBC-slow_cut_passes:


Slow cut passes
===============



:Type:	Integer	
:Range:	{-1 .. 2000000}	
:Default:	10	



This option controls the depth in the branch-and-cut tree at which to do cuts. Cut generators may be off, or switched on only at the root, or switched on if they look useful, or switched on at some interval. Cuts are added whenever the depth in the tree is a multiple of k where k is the value of this option. The default value of -1 means "off".



This option determines the number of rounds that slow cut generators should be applied. The idea is that the code does these cuts just a few times - less than the more usual cuts. The cut generators identiﬁed by ”may be slow” are **Lift and Project Cuts**  and **Reduce and Split Cuts** .



**Learn more about** 

*	:ref:`option-CBC-lift_and_project_cuts`  
*	:ref:`option-CBC-reduce_and_split_cuts`  
