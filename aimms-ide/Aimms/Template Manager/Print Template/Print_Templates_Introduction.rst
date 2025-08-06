

.. _Template-Manager_Print_Templates_Introduction:


Print Templates - Introduction
==============================

**Description** 

AIMMS makes a distinction between end-user pages that are designed for interactive use by the end-user of your application and print pages that are specifically designed for printing on paper. Print pages are characterized by the fact that they depend on a special print template in the template tree. A print template defines a paper type, consisting of a paper size, orientation (portrait or landscape) and print margins. All print pages and normal templates that are placed below such a print template are then specifically designed for that paper type.

You can print normal end-user pages, but these pages will be printed as a bitmap screen dump, so any data that is currently not visible on the page is also not printed. One of the major advantages of print pages is that you can create a printed report in which objects with large amounts of data are automatically resized and/or continued on a next output page. As on normal end-user pages, you can create resizable print pages by adding resize split lines to your print page. However, in a print page you do not create a resizing mechanism to deal with changes in the page size, but merely to changes in the object size (i.e. the minimal required size for an object to display all contained data).



**How to …** 

*	:ref:`Template-Manager_Creating_a_Print_Template` 
*	:ref:`Template-Manager_Linking_Pages_to_Templates` 




**Learn more about** 

*	 Search for Creating printed reports (User's Guide)
*	:ref:`Page-Manager_Resizability_Introduction`  
*	:ref:`Template-Manager_Resizability_and_Print_Templat`  
*	:ref:`Template-Manager_Print_Template_Paper_Type`  
*	:ref:`Shared-Object-Properties_Object_Properties_-_Miscellane`  
*	:ref:`Template-Manager_Template_-_Introduction`  
*	:ref:`Page-Manager_Page_Properties`  



