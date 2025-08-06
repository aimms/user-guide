

.. _Template-Manager_Template_-_Introduction:


Template - Introduction
=======================

**Description** 

Page Templates are used to share specific properties and page objects between pages. Using templates you can create pages with the same look-and-feel, and make it easier to maintain a large number of similar pages. Usually, you create templates to define the basic structure of your pages, such as:

- setting up a default coloring scheme

- creating areas for the title, buttons, a logo, etc.

- adding standard buttons to navigate through the pages.

The templates and pages in AIMMS can be organized in a hierarchical (tree) structure which is maintained in the Template Manager. By simply placing a page (or template) underneath a template (as a 'child' of the template) that page (or template) will inherit the properties and page objects that are defined for that template.



Templates are constructed in the same way as pages. You can open a template from the Template Manager and edit its properties and page objects using the standard page editing tools. If you open a page (or template) for editing, then you can only edit the objects that are not inherited. In fact, you can not even select the inherited objects.



**Remark** 

Although an object may be inherited from a template, its appearance and actions are always based upon the page it appears on. In other words, if you create a button with a Goto Previous Page or Goto Next Page action, then this action is related to the actual page and not the template. Similarly, you can inherit a navigation object that shows the pages relative to the actual page and not its originating template.



**How to …** 

*	:ref:`Template-Manager_Linking_Pages_to_Templates`  
*	:ref:`Template-Manager_Creating_a_Template`  
*	:ref:`Navigation_Navigation_Object_Creating`  




**Learn more about** 

*	 Search for Pages and page objects (User's Guide)
*	:ref:`Page-Manager_Page_Introduction`  
*	:ref:`Template-Manager_Template_Manager_Introduction`  



