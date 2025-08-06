

.. _Gantt-Chart_Gantt_Chart_-_Real-time_Calend:


Real-time Calendar
==================

**Description** 

The calendar X-axis consists of one or more rows and each of these rows corresponds to a specific calendar unit. For example, you can create three rows in which the top rows displays the day numbers within the month, the second row the names of each month, and the third row the year. Using the list box on the X-axis tab, you can select which units you want to display and in which order.



To link the calendar correctly to your model data, you need to specify at least the Unit of Measurement, and a Reference time:



**Unit of Measurement** 

If your original range is continuous, then you should specify how a value of 1.0 of the numerical Start identifier is translated into calendar units (for example 12 hours, 5 days, 1 year, etc). It is assumed that the Duration identifier uses this same unit.



If your original range is discrete, then you should specify the 'length' of a single element in the set. For example, if you specify 5 days, then that part of the X-axis that originally showed one element of the set will now be translated into a period of 5 days.



**Reference time** 

If your original range is continuous, then you should specify the calendar time that corresponds to the 0.0 value of the start identifier.



If your original range is discrete, then you should specify the calendar time that corresponds to the 'left' side of the first element in the root set.



The reference time should be specified using the default AIMMS time format: "YYYY-MM-DD hh:mm:ss". You can enter this string directly or use a string parameter from the model.



**Left bound / Right bound** 

In these fields you can specify which part of the calendar should be currently visible. These bounds should also be presented in the default time format, using either a static string, or a string parameter. When using a string parameter, you can influence the currently visible part of the Gantt chart from within your model.

If you use static strings or not string parameters that are not updatable, then you no longer scroll the Gantt chart to the left or right.



**Week Day Set / Month Set** 

If one of the calendar rows uses the names of weekdays or months, then you can use these two fields to specify alternative names (other language). You can specify a set name, in which the elements consist of the alternative names.



**Start / Duration** 

When using a calendar in combination with a status line, then you can specify here which time format should be used to display the start time and duration of the currently selected bar in the chart. This only works if the start time and duration parameters have a unit associated with them.



**Ignore Daylight Saving Time** 

With this option you can specify whether or not the Gantt chart should apply the Daylight Saving Time in its calendar. If Daylight Saving Time is applied, the calendar will be displayed such that, when entering Daylight Saving Time the day really looks an hour shorter, and when leaving Daylight Saving Time the day looks an hour longer.

