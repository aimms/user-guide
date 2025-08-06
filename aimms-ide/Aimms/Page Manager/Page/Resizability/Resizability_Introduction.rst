

.. _Page-Manager_Resizability_Introduction:


Resizability Introduction
=========================

**Description** 

Initially a page in AIMMS in not resizable, which means that all objects will always keep the same size and remain on the same position relative to the top-left corner of the page, regardless of the size of the page. If you decrease the size of such a page, AIMMS will automatically add horizontal or vertical scrollbars when needed, and if you increase the size of a page the right and bottom parts will remain empty.

In a resizable page, you can define how the objects on a page should be resized and repositioned whenever the page size is changed. To create a resizable page, you must place at least one so-called split line on the page. These split lines can be added when the page is in Resize Edit mode.

You can place both horizontal and vertical split lines on a page. Each split line divides the rectangle in which it is placed into two sub-rectangles (which in turn can be split further). There are several types of split lines, having different rules for how the sub-rectangles on either side of the split line should respond to a change in size of the surrounding rectangle.



**Remark** 

You should be a little careful in how you position the split lines and the page objects relative to each other. Although every combination is accepted by AIMMS, you can create a resize scheme in which resizing the page results in a situation where objects are no longer properly aligned or even overlap each other.

To make sure that objects are resized and repositioned correctly:

*	If a split line crosses an object, then it should cross the entire object, otherwise
*	(if a split line stops at another split line somewhere in the middle of an object) create a similar split line at the other side of that line. In other words: avoid T-crossings of split lines in the middle of an object.

To check how the split lines affect the objects, you can use the Resize Try mode of a page.





**How to…** 

*	:ref:`Page-Manager_Creating_a_Split_Line` 
*	:ref:`Page-Manager_Removing_a_Split_Line` 
*	:ref:`Page-Manager_Moving_a_Split_Line` 




**Learn more about** 

*	:ref:`Page-Manager_Split_Line_Properties`  
*	:ref:`Page-Manager_Resize_Try_Mode`  



