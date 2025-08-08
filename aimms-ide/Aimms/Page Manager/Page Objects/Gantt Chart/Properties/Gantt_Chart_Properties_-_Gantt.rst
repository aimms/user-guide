

.. _Gantt-Chart_Gantt_Chart_Properties_-_Gantt:


Gantt Chart
===========

**Description** 

The Gantt chart property tab contains properties that are specific to the Gantt chart. 



**Legend** 

A Legend above the chart can show you which color corresponds to which identifier. As a default every set of task data has one color. This can be changed using the legend domain.



**Y Labels** 

You can choose to display the labels in the row domain on the y-axis.



**X Labels** 

You can choose to display labels when you use an element start parameter.



**Vertical Grid** 

This option controls whether or not vertical grid lines are shown. The number of gridlines shown depends on the type of X-axis.



**Status Line** 

This options controls whether or not a status line is displayed. The status line is the area at the bottom of the object in which the value and description of the currently selected bar (task) is shown. 



**Store Selection in** 

The identifier that you fill in here can be used within the model to keep track of which bars are currently selected. You should enter a numerical model identifier with the same domain as the task data. This identifier will get the value of 0 for those indices that correspond to bars that are not selected. The identifier will get the value of 1 for the indices corresponding to the currently selected bar. The identifier will get the value of 2 for indices corresponding to any other bar that is part of the selection.



**Show Inactive Data** 

If this option is not selected, inactive data will be considered to have a default value. In the Gantt chart this means, for example, that there no bar will be drawn for an inactive element in the Domain identifier. You can read more about inactive data in the Language Reference.



**Learn more about** 

*	 :ref:`inactive_data`



