

.. _Gantt-Chart_Gantt_Chart_Identifiers:


Gantt Chart Identifiers
=======================

**Description** 

To create a Gantt Chart in AIMMS you need to specify the Task Data, which consists of three identifiers from the model:

1) An identifier representing the start time of a task

2) An identifier representing the duration of a task, and

3) An identifier to indicate which tasks are to be shown, and what resources it uses (the 'index domain' of the Gantt chart)

In addition to this, you can (optionally) indicate which resource you want to display as the rows in the Gantt chart, and/or which resource you want to represent using the legend colors.





Example:



``Start`` ``:`` 	``start_time( person, task )`` 

``Duration`` ``:`` 	``duration( task )`` 

``Domain`` ``:`` 	``resource_assignment( person, task, machine )`` 



``Row index`` ``:`` 		``person`` 

``Legend index`` ``:`` 	``machine`` 





To draw the individual bars, AIMMS uses these identifiers in the following manner:

For each non-default tuple ('person_i', 'task_j', 'machine_k') of the identifier resource_assignment, AIMMS will get the start time from start_time('person_i',task_j') and the duration from duration('task_j'). It will then draw a bar on the row representing 'person_i' using the color that corresponds to 'machine_k'. 



In this example we choose to let the duration only depend on the task, and the start depend on the combination of person and task. In fact, you can use any subset of the indices that are part of the domain identifier, or specify a scalar identifier or a fixed value.



When creating a Gantt chart, you can only specify one group of task data. Once created, you can add other groups of task data via the Contents tab of the Properties dialog box.



**Discrete versus Continuous Gantt charts** 

AIMMS supports two main types of Gantt charts, which differ in how the time along the X-axis is presented (either via a continuous numerical range or via elements from a time set). Which one you use depends on how your model deals with time.



If your model uses a (finite) time set (for example: { day1, .., day100 } ), then the start of a specific task will probably correspond to an element in this set, and the length of a task is measured in multiples (or fractions) of these elements. You can use this representation directly in a discrete Gantt chart. The x-axis of a discrete Gantt chart shows the elements of the time set.

AIMMS automatically assumes a discrete time representation, when an element parameter is filled in as Start identifier.



If your model uses a continuous time frame, then the start and length of a task should be numerical identifiers. This results in a continuous Gantt chart. The x-axis of a continuous Gantt chart shows a value range, similar as the Y-axis range of a curve or bar chart.



If you combine multiple groups of task data in the same Gantt chart, then these groups should either be all discrete (using the same time set) or all continuous.



**Note** 

*	In a discrete Gantt chart, the task duration is measured in multiples (of fractions) of elements. If you want the user to be able to modify the duration via a drag operation, but you do not want him to create fractional duration, you should use a duration identifier with an integer range.




**Tips & Tricks** 


By using a special combination of task data, you can create a Gantt chart that looks like a bar chart with horizontal bars instead of vertical bars:





``Start`` ``:`` 	``0.0`` 


``Duration`` ``:`` 	``Length(i)`` 


``Domain`` ``:`` 	``i`` 





``Row index`` ``:`` 	``i`` 





By adding a second group of task data to the Gantt chart above, you can even create a 'stacked' horizontal bar chart





``Start`` ``:`` 	``0.0`` 


``Duration`` ``:`` 	``Length(i)`` 


``Domain`` ``:`` 	``i`` 





``Row index`` ``:`` 	``i`` 





 	+





``Start`` ``:`` 	``Length(i)`` 


``Duration`` ``:`` 	``Size(i)`` 


``Domain`` ``:`` 	``i`` 




