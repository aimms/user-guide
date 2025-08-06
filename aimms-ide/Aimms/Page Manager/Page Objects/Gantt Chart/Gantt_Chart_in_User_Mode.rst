

.. _Gantt-Chart_Gantt_Chart_in_User_Mode:


User Mode
=========

**Description** 

In user mode you can make changes to a Gantt chart by dragging the bars in the Gantt chart.

The Gantt chart offers several possible dragging operations on the bars (representing a task), but whether or not all of them are allowed depends on the type of Task Data that is used:

1.	If you click and drag the right side of a bar, then you can change the length of the bar (task duration).

2.	If you click and drag on the left side of a bar, then you can change both the start position and the length of a bar, while keeping the end position on the same place.

3.	If you click and drag any other part of the bar, then you can move the bar to a new start position (horizontally or vertically) without changing its length.



All these dragging operations (except the vertical move) can also be applied on multiple selected bars.



Restrictions

*	Moving the start position of a bar is only allowed if the Start identifier is updatable.
*	Changing the length of a bar is only allowed if the Duration identifier is updatable.
*	Changing the vertical position of a bar is only allowed if the row index is NOT used in either the Start identifier or the Duration identifier.




**Note** 

*	You can only change the value of an identifier if the Gantt chart is not read-only and if the identifier is in the set CurrentInputs, which generally means that the identifier should not have a definition.




**How to ...** 

*	:ref:`Model-Explorer_Cut_Copy_Paste_and_Delete`  
*	:ref:`Miscellaneous_Undo_Edit`  




**Learn more about** 

*	:ref:`Gantt-Chart_Gantt_Chart_Introduction`  



