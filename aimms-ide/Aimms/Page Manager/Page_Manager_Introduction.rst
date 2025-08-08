

.. _Page-Manager_Page_Manager_Introduction:


Page Manager Introduction
=========================

**Description** 

In large decision support systems with many pages, navigating your end-users in a consistent manner through all end-user screens becomes an important part of setting up your application. The pages can be organized in several clear structures such as a simple wheel structure for applications with relatively few pages, or a layered setup in projects where a large number of pages is present. The division of pages in sections and subsections can help the end-user to keep a good overview of his position in the interface. To help setting up—and modifying—such navigational structures quickly and easily, AIMMS offers the Page Manager. With the Page Manager you can organize all existing pages in an AIMMS application in a tree-like fashion. The tree in the Page Manager holding all pages is called the Page Tree. Relative to a particular page in the Page Tree, the positions of the other pages define common page relationships such as parent page, child page, next page or previous page. 



Based on the hierarchy of pages in the Page Manager, AIMMS offers several navigational interface components that can be added to a page or end-user menu such as Navigation Objects, Navigation Menus and Button Actions. These components allow for an easy navigation to the parent, child, next or previous pages with respect to either the current page or a fixed page in the page tree.



The power of the Page Manager lies in the fact that it makes it easy to add or delete a page, or to modify the order of navigation without the need to make modifications to the pages themselves. Thus, when a model adjustment requires a new section of pages, you only need to construct these pages, and store them at the appropriate position in the page tree. With the proper navigational interface components added to the parent page, the new pages in the section are then automatically available to the end-user (without any modification of existing pages).



In addition to permanently modifying the page tree, you can also specify that a page be hidden dynamically based on an identifier in your model. Hidden pages are automatically excluded from all navigational interface components referring to the page, effectively disallowing any access to it. 



For larger applications, end-users can usually be divided into groups of users possessing different levels of authorization within the application. Disabling pages based on the level of authorization of the current user then forms a common way to prevent users from accessing those data to which they should not have access.



**How to …** 

*	:ref:`Page-Manager_Opening_the_Page_Manager`  




**Learn more about** 

*	:ref:`Page-Manager_Page_Introduction`  
*	:ref:`Page-Manager_Manipulating_the_Page_Navigati`  
*	:ref:`Page-Manager_Page_Navigation`  
*	:ref:`Page-Manager_Maintaining_Pages_and_Template`  
*	:ref:`Page-Manager_Page_Manager_-_Menubar`  
*	:ref:`Page-Manager_Page_Manager_-_Toolbar`  
