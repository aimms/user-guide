

.. _Miscellaneous_Localization_Setup:


Setup
=====

**Description** 

Before you can use the localization conversion and text wizard of AIMMS you have to run the Localization-Setup command from the Tools menu.

If you have already executed this command before, a dialog box appears in which you can change any of the localization identifiers, but usually the current setup needs not be changed. If you run the command for the first time, the Setup process will add a special section, called Localization, to your model (and each of your Library Modules). This section contains the necessary declarations for using localization tools in your project. If you want to know more about the individual declaration in this section you can read the comments that are added to each identifier and procedure, or you should refer to the corresponding chapter in the Users Guide.



In a project with multiple libraries, it is recommended to have a Localization section in each separate (library)project. This makes it easier for multiple developers to modify their library, because there is then no need to have write access to the main project.



**Learn more about** 

*	 Search for Localization (User's Guide)



