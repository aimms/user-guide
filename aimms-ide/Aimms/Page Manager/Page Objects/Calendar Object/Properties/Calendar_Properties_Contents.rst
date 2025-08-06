

.. _Calendar-Object_Calendar_Properties_Contents:


Contents
========

**Description** 

This tab contains the properties that specify to what AIMMS identifiers the calendar is linked.



**Begin date** 

This property is required. You must select the AIMMS identifier that will hold the selected date (or the first selected date, in case you select a date range). The AIMMS identifier should be either a string parameter or an element parameter into an AIMMS calendar set. If you specify a string parameter, it will have the default AIMMS date format when filled.



**End date** 

This property is only required when the property "Max. number of dates" has a value greater than 1. You can specify the AIMMS identifier that will hold the last date of a selected date range. See the "Begin date" property for valid AIMMS identifiers.



If "Max. number of dates" is 1 (its default value), you are still allowed to specify this property. In that case, upon selecting a date, both the identifiers specified for "Begin date" and "End date" will be filled with the same value.



**First date allowed** 

This property specifies the minimum date that the user is allowed to select from the calendar. The calendar doesn't show months before the month in which the first allowed date lies. You can specify an element into an AIMMS calendar set, a string parameter or a literal string. In the latter two cases, the standard AIMMS date format should be used (this includes a time component!).



**Last date allowed** 

This property specifies the maximum date that the user is allowed to select from the calendar. The calendar doesn't show months after the month in which the last allowed date lies. You can specify an element into an AIMMS calendar set, a string parameter or a literal string. In the latter two cases, the standard AIMMS date format should be used (this includes a time component!).



**Max. number of dates** 

This property specifies the maximum number of dates that are allowed in a selection. The default is 1.



**Procedures subtree** 

The procedures subtree contains the properties to link AIMMS procedures to the calendar. Currently, only one such property is implemented.



**On change** 

This property specifies which AIMMS procedure should be executed when the selection in the calendar changes.





