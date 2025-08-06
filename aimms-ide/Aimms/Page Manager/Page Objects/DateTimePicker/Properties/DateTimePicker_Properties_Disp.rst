

.. _DateTimePicker_DateTimePicker_Properties_Disp:


Display
=======

**Description** 

This tab contains all properties needed to control the way the object is displayed on the page.



**Font** 

This property specifies the font to use for displaying both the date/time box and the calendar used for picking a date.



**Control type** 

This property specifies the way in which the user can select a date/time through the object. The valid values are "Dropdown calendar" (default) and "Spin button". The value "Dropdown calendar" has the effect that when the user clicks on the dropdown button to the right of the object, a calendar will appear, through which the date can be selected. The value "Spin button" results in a spin button to appear to the right of the object, with which the user can spin the selected part of the date/time up or down.



To select the part of the date/time to spin, just click on it in the object. You can also spin the date/time using the arrow keys after having selected a part. This can be done, regardless of the control type selected.



**Date format subtree** 

This subtree contains the properties needed to control the date/time format of the date/time that is displayed in the object.



**Use predefined date/time format** 

**There are two ways of specifying the date/time format. The first way is exclusively used in AIMMS versions prior to 3.9. This uses some predefined date/time formats, which you can choose from. The second way has been introduced in AIMMS version 3.9. This gives the user a bit more flexibility in specifying the date/time format, while at the same time being more in the style of date/time handling throughout AIMMS.** 



**Specifying "Yes" for this option, selects the first way of specifying the date/time format. Specifying "No" selects the second way. In the latter case, only one additional option must be specified and the options from "Day/month name" on are hidden in the property tree.** 



**Custom date/time format** 

With this option, which is only displayed when you have specified "No" for the option "Use predefined date/time format", you can specify a custom date/time format to be used for displaying the date/time in the Date Time Picker control. This custom format should be entered as either a literal string, or a string parameter from your model. In this string (parameter), the following placeholders can be used to control the displaying of date/time related fields:



**%c** 

Displays the century (e.g. '20' for the year 2008)



**%y** 

Displays the year in the century (e.g. '08' for the year 2008)



**%m** 

Displays the month number (e.g. '11' for November)



**%d** 

Displays the day number (e.g. '07' for November, 7th)



**%h** 

Displays the hour in 12-hour format (e.g. '11' for 23:00)



**%H** 

Displays the hour in 24-hour format (e.g. '23' for 23:00)



**%M** 

Displays the minutes (e.g. '00' for 23:00)



**%S** 

Displays the seconds (e.g. '05' for 23:00:05)



**%p** 

Displays either 'AM' or 'PM', according to the currently displayed time



``%Am|AllMonths|`` 

Displays the full (English) name of the month (e.g. 'November')



``%Am|AllAbbrMonths|`` 

Displays the abbreviated (English) name of the month (e.g. 'Nov')



``%Aw|AllWeekdays|`` 

Displays the full (English) name of the week day (e.g. 'Saturday')



``%Aw|AllAbbrWeekdays|`` 

Displays the abbreviated (English) name of the week day (e.g. 'Sat')



Placing the 's' modifier between the percentage sign and the placeholder character(s), for all characters except 'p' and the month- and week name placeholders, has the result that leading zeroes are not displayed.



Furthermore, the following characters can be used in the string: -()[]{}.':;/<>



``As an example, the string "%Aw|AllWeekdays| %d/%m/%c%y %h:%M:%sS %p" will display "Saturday 29/11/2008 10:59:1 PM" for November 29th, 2008, 22:59:01.`` 



If you specify an illegal date/time format by means of a string parameter (runtime), the text 'Illegal format' will appear in the object, instead of a date/time.



**Day/month name** 

This property and the following properties are only displayed in case "Yes" has been specified for the option "Use predefined date/time format".It specifies the format of the day and month name part of the date. You can choose one of the nine possible values, which are listed in the popup menu that appears when you click on the icon to the right of the property. The nine values are all nine possible combinations of:



the full day name (denoted by "Monday" in the menu)

a three-letter abbreviation of the day name (denoted by "Mon" in the menu)

no day name at all (denoted by "(None)" in the menu)



on the one hand, and of:



the full month name (denoted by "January" in the menu)

a three-letter abbreviation of the month name (denoted by "Jan" in the menu)

the number of the month (denoted by "1" in the menu)



on the other hand.



**Date format** 

Depending on the value specified for the "Day/month name" property, you can specify one of many valid complete date formats for this property. The date format is split in two properties ("Day/month name" and "Date format") to keep the lists of possible values in the popup menus surveyable.



**Time format subtree** 

The "Time format" subtree contains the properties with which you can specify the time format. Again, the time format is specified through more than one property, in order to keep the list(s) of possible values surveyable.



**Show time component** 

This property specified whether you want to show a time component at all. The default value is "No", while "Yes" is the other allowed value. If you select "Yes", the next three properties become visible.



**Hour format** 

With this property, you can select the hour format to use for the time component. You can choose from one of the possible values "24-hour" (the default) and "AM/PM".



**Show hour leading zero** 

Set this property to "Yes" if you want to show a leading zero before hours that only consist of one digit. If not, leave the property on its default value "No".



**Show seconds** 

This property specified whether you want the time component to include seconds. If so, specify the value "Yes". If not, specify the value "No" (the default).





