

.. _Page-Manager_Split_Line_Properties:


Split Line Properties
=====================

**Description** 

For both horizontal and vertical split lines, there are three different types of lines:



**Percentage from Top/Left** 

The line will remain on a fixed percentage from the current width/height of the rectangle it is created in. This means that if a rectangle with such a split line grows with a factor n then the rectangles on both sides of the line grow with that same factor. You can specify the percentage in the edit field below the radio button choices.



**Fixed Distance from Top/Left (or Bottom/Right)** 

A Fixed Distance split line is attached to one of the four borders of a rectangle and remains on a fixed number of pixels from that border. This type of line implicitly imposes a minimum size on the rectangle it splits up. You can specify the number of pixels to be maintained in the edit field below the radio buttons.



**Adjustable Distance from Top/Left (or Bottom/Right)** 

An Adjustable Distance split line is initially similar to a Fixed Distance split line, but these lines are visible when the page is in User mode. The End-User himself can drag these lines to new positions. Additionally, he can double-click the line to let the system determine the 'optimal' position of the line. For example, if a adjustable horizontal split line is attached "to the top", then, if you double-click on that line, for each object above that line AIMMS will calculate the minimal needed area so that all data in that object is visible (without the need for scroll bars), and then try to re-position the split line so that these minimal areas are available for these objects.

You can specify the number of pixels to be maintained in the edit field below the radio buttons.



**Remark** 

In the Resize Edit Mode the split lines have different colors, corresponding to different properties. The Percentage split lines are black, the Fixed Distance split lines are red and the Adjustable Distance split lines are blue,



**How to…** 

*	:ref:`Page-Manager_Changing_the_Property_of_a_Spl` 



