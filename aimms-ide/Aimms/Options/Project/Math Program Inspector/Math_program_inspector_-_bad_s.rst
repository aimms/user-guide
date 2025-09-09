

.. _option-AIMMS-bad_scaling_threshold:


Bad Scaling Threshold
=====================



:Type:	Selection	
:Range:	[10,1e9]	
:Default:	1000	



The colors of the displayed blocks on the Matrix View tab of the Math Program Inspector window correspond to the value of the coefficient. The colors will vary between green and red indicating small and large values. Any number with absolute value equal to one will be colored green. Any number for which the absolute value of the logarithm of the value exceeds the logarithm of the 'bad scaling threshold' value will be colored red.



By default, the threshold is set to 1000, meaning that all nonzeros x in (-inf,-1000] union [-1/1000,1/1000] union [1000,inf) will be colored red. All numbers in between will be colored with a gradient color in the spectrum between green and red. In symbolic mode the worse value of all coefficient that correspond to the symbolic block will be responsible for the color of the block.



**Learn more about** 

*	:ref:`Math Program Inspector <aimmshelp26-Math_Program_Inspector>`  






