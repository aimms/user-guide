

.. _Miscellaneous_File_Printing:


File Printing
=============

**Description** 

AIMMS offers two distinct facilities to create printed reports associated with your model, namely prints of graphical end-user and print pages, and prints of text files such as the ASCII representation of a part of the model tree or the listing, log and PUT files. This section explains how you can configure the printing properties for both types of reports. End-user pages and print pages are printed according to the settings that you have selected for these pages. These settings include:

*	The selection of the paper type on which pages are printed.
*	The selection of object fonts and colors through the AIMMS font and color selection dialog boxes.

These settings must be determined by you as the application developer, and cannot be changed by an end-user of your application. An end-user can, however, still select the printer to which the output must be send, as explained below.


Text files can be printed from within AIMMS either by means of the File-Print menu inside an AIMMS text editor window, or through a call to the FilePrint procedure from within a procedure in your model. The print properties of all text files that you want to print in either manner can be modified through the Settings-Text Printing menu. The dialog box that appears upon calling this menu item has the same functionality as the Page Type dialog box of a print template plus the option to select the font, which you want your text files to be printed in, in a standard Windows font selection dialog box. The text printing properties are stored globally on your machine.


With the File-Print Setup menu you can select the printer to which print pages and text files associated with your project are printed, and modify the properties of that printer. This command will invoke the standard Windows print setup. 


The settings selected in this dialog box will only be valid during the current session of AIMMS. If you want to modify the default print setup globally, you can do this via the Printer section in the Windows Control Panel. There you can 

*	select a Default printer from the list of all printers available on your system.
*	modify the Document Defaults(i.e. the printer settings with which each print job is printed by default) for every individual printer on your system.

Without calling the File-Print Setup dialog box, AIMMS will use the default printer selected here, and print according to the document defaults of that printer.





**Learn more about** 

*	:ref:`Template-Manager_Print_Templates_Introduction`  



