

.. _Network_Network_Object_Properties_-_Ne:


Network
=======

**Description** 

In the Network tab of the Network Object Properties dialog box, you can alter the visible area and the drawing order of the object.



**Visible Area** 

The properties in the Visible Area define which part of the network you will currently see on the page.

*	Left, Right, Top, Bottom. These four fields can contain either values or identifiers. If they contain values, the values are used as initial values for the x and y coordinates of what part of the network will be displayed on the page. If the fields contain identifiers, not only will they be used as initial values, but also if the range is changed (either by scrolling or zooming,) the values of the identifiers will change to the new coordinates.




*   **Scrolling & Zooming** 

Here you specify how you can scroll and/or zoom the visible area of the Network Object. The Network Object offers two styles for scrolling (or no scrolling/zooming at all):


1.	**Using Navigation Buttons** , in the corners and along the sides of the object 8 buttons are displayed to scroll in the given direction.


2.	**Using Scroll Bars** , a horizontal and/or a vertical scrollbar is displayed which enables the user to scroll in either direction


3.	**No Scrolling** , no scrolling controls available. The visible area is fixed and can only be changed by altering the Left, Right, Top or Bottom values programmatically. 





*   **Draw Buttons Transparent**  (only if 'Using Navigation Buttons' is selected). The 8 navigation buttons (and the 2 zoom buttons) at the borders of the object are drawn transparent, instead of using the standard button color.
*   Horizontal/Vertical Scrollbar (only if 'Using Scroll Bars' is selected). If you want to able to scroll only in one direction, you can uncheck one of these checkboxes.

*	Zoom Allowed. This checkbox specifies whether it is possible to zoom on the network. If this option is selected the user can drag areas in the object to zoom into.
*	Equal X and Y scale and Automatic Adjust. With this option you can make sure that the visible area cannot be stretched in only one direction, for example if the horizontal range of the visible area changes, then the vertical range will also change. Which of the ranges will automatically be adjusted can be specified in the Automatic Adjust field.




**Drawing Order** 


This property contains a field that specifies whether first arcs or first nodes should be drawn. This is important in case of overlapping.





**Show Inactive Data** 


If this option is not selected, inactive data will be considered to have a default value. In the Network object this means that no arc is drawn for an inactive element tuple of an arc identifier. You can read more about inactive data in the Language Reference.








**Tips & Tricks** 

*	If you specify four scalar identifiers for the Left, Right, Top and Bottom, then you can write procedures that handle your own specific scrolling or zooming of the visible area.




**Learn more about** 

*	 :ref:`inactive_data`






