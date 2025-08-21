

.. _Miscellaneous_Saving_and_Restoring_Layouts:


Saving and Restoring Layouts
============================



The AIMMS IDE can save the layout of the currently opened docked (and floating) windows, such that when you re-open the project, you come back to the same layout as when you left.



By default, the layout is saved when closing the project, and this layout is restored upon re-opening the project. Via the option :ref:`option-AIMMS-startup_layout` you can change this default behavior, for example to make sure that an end-user application always starts with a default (developer defined) layout.



How and when a layout is saved and restored, depends on the setting of the option :ref:`option-AIMMS-startup_layout`. This option has three possible values: 'Last use', 'From project' and 'System default'.



**Saving** 

If the option Startup Layout is set to 'Last use' then the End-User (and Developer) layout is saved when you close the project. It does not depend on whether or not you saved the project, and thus also works when running the End-User version of AIMMS. However, in the End-User version only the End-User layout is saved.

These 'Last use' layouts are stored in the Registry of your computer using the full path of the .prj file as the key. This layout is thus only used for the current user, and the current location of the .prj file. If you copy or move the project to another location (or other computer), this layout will not be restored.



If the option Startup Layout is set to 'From project', then you must save a layout explicitly via the menu command **Window - Layout - Save Layouts to Project** . This layout becomes part of the .prj file and thus can be re-used when the project is copied. Only a developer with write access on the .prj file, can change this layout. If you use this setting, then an End-User of your application will always start from the End-User layout that the developer has created, and the changes to the layout made by the End-User during a session are lost upon closing.



If the option Startup Layout is set to 'System default', then specific layouts are not saved or restored, and the project will always start with a default layout. The default Developer layout consists of only a visible Model Explorer and Page Manager, the default End-User layout will not open any docked window at startup.



**Restoring** 

When re-opening a project, AIMMS tries to restore the End-User and/or Developer layout using the following sequence:




#.   If the option Startup Layout is set to 'Last use', then the registry is searched for an existing layout, using the full path name of the .prj file as a key. If no layout can be found, or if the layout cannot be loaded successfully, the sequence proceeds as if 'From project' is set.




#.   If the option is set to 'From project', then AIMMS will try to read the layout from the .prj file. If no layout has yet been saved in the .prj file, or if the layout cannot be loaded successfully, the sequence proceeds as if 'System default' is set.




#.   If the option is set to 'System default', then the system-defined layout is loaded which is the same for all projects.



**Reset** 

While working in the IDE you can open various docking windows and arrange them in any way you want. If you feel that you have changed the layout too much and perhaps don't feel comfortable in changing things back, you can also use the menu command **Window - Layout - Reset to Default** . 



If the option Startup Layout is not set to 'System default' and the project file contains a saved layout, this command will restore the layout present in the project file. Otherwise, the system default layout will be restored.



