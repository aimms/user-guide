

.. _Diagnostic-Tools_Math_Program_Inspector_Matrix1:


Matrix View
===========

**Description** 

By selecting Matrix View from the View menu, the Matrix View tab is opened. This tab contains a graphical representation of the generated matrix. The part of the matrix that is shown is restricted by the selections in the variable and constraint tree. The Matrix View is available in two modes that are accessible through the right-mouse popup menu. The symbolic block view displays at most one block for every combination of symbolic variables and symbolic constraints. The individual block view allows you to zoom in on the symbolic view and displays a block for every nonzero coefficient in the matrix.



**Block coloring** 

The colors of the displayed blocks correspond to the value of the coefficient. The colors will vary between green and red indicating small and large values. Any number with absolute value equal to one will be colored green. Any number for which the absolute value of the logarithm of the value exceeds the logarithm of some threshold value will be colored red. By default, the threshold is set to 1000, meaning that all nonzeros x ÎÎ (-¥¥, -1000] ÈÈ [-1/1000,.1/1000] ÈÈ [1000, ¥¥) will be colored red. All numbers in between will be colored with a gradient color in the spectrum between green and red. The value of the threshold is available as an AIMMS option with name bad_scaling_threshold and can be found in the Project - Math program inspector category in the Aimms Options dialog box.



**Block tooltips** 

While holding the mouse inside a block, a tooltip will appear displaying the corresponding variables and constraints. In the symbolic view the tooltip will also contain the number of nonzeros that appear in the selected block. In the individual view the actual value of the corresponding coefficient is displayed.



**Block view features** 

Having selected a block in the block view you can use the right-mouse popup menu to synchronize the trees with the selected block. As a result, the current bookmarks will be erased and the corresponding selection in the trees will be bookmarked. Double-clicking on a block in symbolic mode will zoom in and display the selected block in individual mode. Double-clicking on a block in individual mode will center the display around the mouse.



**Learn more about** 

*	 Search for AIMMS math program inspector (User's Guide)






