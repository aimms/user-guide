.. |img_def_Identifier_Calendar_bmp| image:: images/Identifier_Calendar.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Calendar:


Creating a Calendar Identifier
==============================

**Description** 

To create a new calendar in the Model Tree:

1.	Select the position in a Declaration Section where the new calendar should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Calendar_bmp| Calendar and press OK

4.	Enter a name for the new calendar

5.	Press ``<Enter>``  to create the new calendar (or press ``<Esc>``  to abort the operation)



The newly created calendar is not yet ready for use, because you should at least specify some mandatory attributes. To modify the attributes of the newly created calendar:

*	Press ``<Enter>``  or double click on the calendar node.




The most commonly used attributes of a calendar identifier are discussed below. 




*	``BEGIN DATE`` : The ``BEGIN DATE``  attribute should be used to specify the start moment of the time range that is considered in the calendar. The |img_def_Wizard_button_bmp| wizard will a display dialog box allowing you to specify a moment in time.
*	``END DATE`` : The ``END DATE``  attribute should be used to specify the end moment of the time range that is considered in the calendar. The |img_def_Wizard_button_bmp| wizard will display a dialog box allowing you to specify a moment in time.
*	``UNIT`` : The ``UNIT``  attribute is mandatory and is used to define the length of a single time slot in the calendar. The |img_def_Wizard_button_bmp| wizard will display a dialog box allowing you to select from one of the available time units.
*	``TIMESLOT FORMAT`` : The ``TIMESLOT FORMAT``  attribute is used to specify the format of the elements in the calendar. The |img_def_Wizard_button_bmp| wizard will allow you to select from various predefined timeslot formats.
*	``INDEX`` : The ``INDEX`` attribute is the place to declare indices in the current calendar. The |img_def_Wizard_button_bmp| wizard allows you to declare new index, delete or rename an existing index or move an index to another set. 
*	``PARAMETER`` : The ``PARAMETER`` attribute is like the ``INDEX``  attribute except that it allows you to declare scalar element parameters (instead of indices) in the current calendar. 




**Remark** 


A calendar is a special kind of set. You can use a calendar to index data defined in terms of calendar time.





**How to ...** 

*	:ref:`Model-Explorer_Creating_a_Set`  




**Learn more about** 


*	:ref:`sec:time.calendar`
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



