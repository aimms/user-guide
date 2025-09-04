

.. _Miscellaneous_Renaming_Libraries_and_Folders:


Renaming Libraries and Folders
==============================

In the :ref:`Miscellaneous_LibraryManager`  dialog box, you can easily add and delete existing or new libraries to your project. However, this dialog box does not (yet) offer features to rename a library.



Nevertheless, it is quite easy to manually rename library folders and let AIMMS work with this new name:



The .aimms file in the root folder of your application contains references to all the libraries that make up your application.



Here is an example of the contents of an .aimms file (assuming the name is ``myAimmsApp.aimms``):



``<?xml version="1.0"?>`` 

``<References AIMMS_Version="4.0.0.400 (x64)">`` 

	``<MainProject Path="MainProject" />`` 

	``<Library Path="MyLibrary1" />`` 

	``<Library Path="MyLibrary2" />`` 

``</References>`` 



This file should resemble the following folder content on your disk:



	``myAimmsApp.aimms`` 

	``MainProject\`` 

		``Project.xml`` 

		``Options.txt`` 

		``MainModel.ams`` 

	``MyLibrary1\`` 

		``Project.xml`` 

		``MyLibrary1.ams`` 

	``MyLibrary2\`` 

		``Project.xml`` 

		``MyLibrary2.ams`` 



If you want to rename the folder ``MyLibrary2`` to ``MySecondLibrary``, you do the rename on disk and you modify the .aimms file accordingly.



Similarly, if you want to rename ``MyLibrary1.ams`` to ``MyFirstLibrary.ams``, you should make a similar modification to the content of the file ``MyLibrary\Project.xml``. 





**Note** 




*   It is recommended that you make these changes when AIMMS is not currently running the project, so exit AIMMS first.
*   Besides the .ams file, most other files in the sub folders have fixed names. So you cannot rename them.



