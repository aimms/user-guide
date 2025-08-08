

.. _Template-Manager_Template_Manager_Introduction:


Template Manager Introduction
================================

**Description** 

Complementary to the Page Manager (and the Page Tree) is the Template Manager (and the Template Tree). Using the Template Manager, you can make sure that all pages have the same size and possess the same look-and-feel. This is done by creating template pages and letting other pages depend on these template pages.

In addition to all end-user pages, the Template Tree can contain a hierarchical structure of template pages. Within the Template Tree, template pages behave as ordinary pages, but they are not available for end-users. Through templates, you can define common page objects that are shared by all pages that descent from the specific template page.

Every new end-user page created in the Page Manager is also automatically added to the root node in the Template Tree. By moving the page in the Template Tree, it will inherit the combined look-and-feel of all templates above it. The hierarchical structure of the Template Tree lets you define layers of common objects on top of each other. Thus, a first template might globally define the page size and background color of all underlying pages, while a second template could define common components such as a uniformly shaped header and footer area. 

You can quickly modify the entire look-and-feel of your application, by moving a subtree of templates and end-user pages from one node in the Template Tree to another. Thus, the entire look-and-feel of page size, header and footer area, background color and navigational area(s) of all pages in an AIMMS application could be changed by a single action.

When you open a template or end-user page in the Template Manager, it will be opened in edit mode by default, and inherit all properties of and all objects contained in the templates above. However, on any template or end-user page you can only modify those objects or properties that are defined on the page itself. To modify objects defined on a template, go to that template and modify the objects there.

An extra powerful combination originates when you add navigational components to a template page. If the reference page property of such a navigational component is expressed relative to the current page, the navigation in end-user mode will also be relative to the current page (i.e. the end-user page that inherits the navigation object). Thus, given a well-structured page tree, you only need a single template to add navigational control components to all end-user pages. This is particularly true for such common controls as Previous and Next buttons.



**Note** 

*	All pages that are contained in the Page Tree will also be present in the Template Tree. On the other hand, template pages will not be displayed in the Page Tree.
*	Similar to the hidden status of a end-user page, you can also make a template page hidden. This means that the objects created on that template are not inherited by (and are not visible on) the pages that descent from it.




**Learn more about** 

*	:ref:`Template-Manager_Template_-_Introduction`  
*	:ref:`Template-Manager_Manipulating_the_Template_Tree`  
*	:ref:`Template-Manager_Object_Overlapping`  
*	:ref:`Template-Manager_Linking_Pages_to_Templates`  
*	:ref:`Template-Manager_Print_Templates_Introduction`  
*	:ref:`Template-Manager_Hidden_Templates`  
*	:ref:`Template-Manager_Template_Manager_-_Menubar`  
*	:ref:`Template-Manager_Template_Manager_-_Toolbar`  



