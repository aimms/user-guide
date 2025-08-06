

.. _Slider_Slider_Properties_Display:


Display
=======

**Description** 

This tab contains the properties that control how the slider object is displayed on your AIMMS page.



**Orientation** 

This property specifies how the slider object is oriented on your page. Valid values are "Horizontal" and "Vertical". By default, the slider object is displayed horizontally.



**Tick properties subtree** 

This subtree contains the properties needed to control the displaying of the ticks (the small lines that indicate the slider positions.



**Tick distance** 

This property controls the distance between every two ticks. By default, the value is 1.



**Tick style** 

This property controls where the ticks should be located, relative to the slider and whether ticks should be displayed at all. The following values are valid:



"No ticks"		: no ticks are displayed at all

"Top/Left"		: the ticks are displayed above the slider in case of a horizontal 

orientation, and to the left of the slider in case of a vertical orientation

"Bottom/Right"		: the ticks are displayed below the slider in case of a horizontal 

orientation, and to the right of the slider in case of a vertical orientation	

"Both"			: the ticks are displayed both above and below the slider in case of

			 a horizontal orientation, and both to the left and to the right of the

			 slider in case of a vertical orientation





**Change properties subtree** 

This subtree contains the properties that control the behavior of the slider object when the user changes the position of the slider.



**Small incr. (arrow keys)** 

This property specifies the number of positions the slider should move in case the user controls it with the arrow keys on the keyboard. The default value is 1.



**Large incr. (PgUp/PgDn keys)** 

This property specifies the number of positions the slider should move in case the user controls it with the PgUp- and PgDn-keys on the keyboard. The default value is 5.



**Update identifier continuously** 

This property specifies when the attached AIMMS identifier is updated. If the value 0 is specified (the default), the AIMMS identifier is only updated when the user has dragged the slider to its final position and has released the mouse or the keys on the keyboard that steer the slider. If the value 1 is specified, the AIMMS identifier is also updated during the dragging process.



Be careful when setting this property to 1. If there are complex definitions of identifiers that depend on the identifier attached to the slider, those definitions will be re-evaluated for every step in the dragging process. This could lead to unnecessarily slow behavior.





