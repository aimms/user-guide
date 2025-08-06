

.. _DateTimePicker_DateTimePicker_Properties_Cont:


Contents
========

**Description** 

On this tab, all properties related to the actual contents of the date/time picker are listed.



**Identifier** 

This property is the most important one: with it, you set the AIMMS identifier that should receive the date/time picked by the user. This can be either a string parameter, or an element parameter into an AIMMS calendar set. If you use a string parameter, the date/time is always passed in the default AIMMS date/time format ("2000-01-01 00:00:00"). If you use an element parameter, the date/time is passed in the format that is specified for the corresponding AIMMS calendar set.



**First date allowed** 

With this property, you can specify the first date of the range of dates from which the user must select one. Either a string parameter with a date/time in the default AIMMS date/time format can be specified, or an element parameter into an AIMMS calendar set.



**Last date allowed** 

With this property, you can specify the last date of the range of dates from which the user must select one. Either a string parameter with a date/time in the default AIMMS date/time format can be specified, or an element parameter into an AIMMS calendar set.



**Procedure Upon Change** 

This property specifies a procedure to be called when a change to the Date Time Picker is made.





