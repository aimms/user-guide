

.. _Miscellaneous_AIMMS_Files:


AIMMS Files
===========

**Description** 

During the development phase of a project, an AIMMS project consists of a set of folders and files on your disk. The main entry point for your application is the .aimms file.

This .aimms file has an XML syntax and its most important content are the references to the Main project and the optional library project(s) that together define your application.



The main project and each additional library is contained in a separate folder. 

This folder typically contains:


*   An .ams :ref:`Miscellaneous_Model_File` ,
*   the file project.xml which, amongst other, defines the name of the project or library, and a reference to the model file,
*   the files PageManager.xml, TemplateManager.xml, and the folders Pages and Templates, which together describe all the pages and template pages created in the project,
*   the file Options.txt, containing the options that are set in the Project Settings dialog,
*   the file MenuBuilder.xml, that contains all user defined menus, menubars and toolbars,
*   the .nch :ref:`Miscellaneous_Name_Change_File` ,
*   and some other folders and files to store the data of the various other tools in the AIMMS IDE.



See also: :ref:`Miscellaneous_Renaming_Libraries_and_Folders` 





**User Files** 

Besides the folders and files that AIMMS itself creates and maintains, your application may need some other folders or files. You cannot put these files in any folder of your application, because during an export these files may not be accessible in the way that you expect, or they are perhaps not exported at all.

If you have your own files that should be distributed together with the project itself, make a separate folder in the same folder where the .aimms file is located and put your files there, such that they are clearly separated from the other files. During the export you can select this folder to become part of the exported project.

Besides creating your own folder, you can also add these files to the :ref:`Miscellaneous_User_Files_in_the_Project_File` .





**.aimmspack files** 

When exporting a project to an End-User project, all the application files and the files that you include explicitly during this step are (encrypted and) put together in a single file with the extension .aimmspack. This .aimmspack is the only file that you need to distribute to your end users.





**The folder .edited** 

While working with the development version of AIMMS on a specific project, you might notice the existence of the folder .edited, next to the .aimms file. This folder is created to temporarily store the changes in components of the UI that are not kept in memory constantly (for example for edits in pages and templates). Only after the command File - Save All, all your edits are actually stored to the folders and files that define your project. It is recommended not to make changes to this folder, because you then might accidentally loose some of the edits that you made.





**Editing the files outside AIMMS** 

Although most of the files are in a text format that can be edited with any ordinary text editor, it is not recommended to do that. Especially not when you have the project still open in AIMMS at that time. AIMMS does not automatically register any changes made to the underlying files, so any external edit will not be directly visible in AIMMS, and might even be overwritten when you do a save in AIMMS.

If you do need to make changes to the files outside AIMMS, make sure that you exit AIMMS first, then make the changes and after that restart AIMMS.

This also holds if you need to synchronize (check in, check out) your files with your version control system!







Optional files:

*	:ref:`Miscellaneous_Startup_Bitmap`  
*	:ref:`Miscellaneous_User_Database_File`  




Output files:

*	:ref:`Miscellaneous_Listing_File`  
*	:ref:`Miscellaneous_Logging_File`  
*	:ref:`Miscellaneous_AIMMS_SIG`  
*	:ref:`Miscellaneous_Solver_Output_Files`  



