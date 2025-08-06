

.. _File-Name_File_Name_Properties_-_File_Na:


File Name
=========

**Description** 

The File Name property tab contains the specific properties that are available for the File Name object. You can adjust the following properties here:



**Default Directory** 

Here you can specify the default directory where the user should select or create a file name. The File Selection dialog box, that is opened when the user click on the button will initialize to this default directory. If not specified, then the current (project) directory will be used.



**Filter** 

If you specify a filter extension, then only the file names with that extension are shown in the File Selection dialog box.



**Allow** 

At the Allow entry you can specify what file names the associated string parameter can contain. This can be one of three possibilities: 

*	Any File Name, no error checking on existence of the file is done.
*	Existing File Name, only existing file names are allowed (usually for reading a file).
*	New File Name, new file names are allowed, and a warning is given if an existing file name is selected (usually for writing a file).




**Remark** 


The File Name object does not create, modify or delete any file on the disk. It only returns a string containing a valid file name. So even though the dialog box may request a confirmation on overwriting existing files, the file is only overwritten when your application starts writing the file. Similarly, any new file name that is selected is only created when your application creates that file.




