

.. _Page-Manager_Resize_Try_Mode:


Resize Try Mode
===============

**Description** 

The Resize Try Mode is the mode in which the effects of the resizability settings of a page can be checked. In this mode both the resize lines and the objects are visualized by simple lines and rectangles. If you resize the page, you can see the effect on the position and sizes of the objects.

In the Resize Try Mode, AIMMS calculates the resized coordinates for all 4 corners of an object, and reshapes the 'rectangle' accordingly. If you do not position the resize lines and objects carefully, this may lead to shapes that are no longer rectangular (these non-rectangular shapes are colored green). The actual page objects cannot have these non-rectangular shapes and therefore, during the normal resizing of page objects in End User mode, AIMMS only calculates the resized coordinates for the top-left and bottom-right corners. This seems to be a reasonable solution, but this may lead to objects that are no longer correctly placed relative to other objects, and even to situations in which objects are overlapping.



To make sure that objects are resized and repositioned correctly:

*	If a split line crosses an object, then it should cross the entire object, otherwise
*	(if a split line stops at another split line somewhere in the middle of an object) create a similar split line at the other side of that line. In other words: avoid T-crossings of split lines in the middle of an object.




To open a page in Resize Try Mode:


1.	Open the page in Resize Edit Mode.


2.	From the View menu, select Resize Try Mode.





**Learn more about** 

*	:ref:`Page-Manager_Resizability_Introduction` 
*	:ref:`Page-Manager_Page_Resize_Try_Mode_-_Menubar` 
*	:ref:`Page-Manager_Page_Resize_Try_Mode_-_Toolbar` 



