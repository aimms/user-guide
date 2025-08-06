

.. _Menu-Builder_Listing_Pages_Associated_with_:


List Pages Associated with Menu Tree Nodes
==========================================

**Description** 

In a similar way as you can use a drag operation to find the identifiers that are used in the Menu Builder, you can also use a drag operation to find all pages and templates that contain one of the menubars, toolbars and popup menus in the Menu Builder.

To find out which pages contain a certain menubar, toolbar, popup menu, menu item or separator.

1.	Open both the Menu Builder and Template Manager.

2.	In the Menu Builder, select the nodes (menubars, toolbars and/or popup menus) you want to search for.

3.	Drag the selection to the tree of the Template Manager.

AIMMS will now highlight all the pages and templates that contain one or more of the selected menu nodes.



**Note** 

*	This drag operation also works for the Page Manager (instead of the Template Manager), but, of course, you will then not find the templates that contain references to the menu nodes.
*	With the drag operation described above, you can find which pages and templates use a specific menu node. Similarly, within a page, you can find all objects that use a specific popup-menu:

1.	Open a page in Edit Mode.


2.	Drag popup menu nodes from the Menu Builder to the page.


All objects that contain the specific popup menu are now selected.





**Learn more about** 

*	:ref:`Page-Manager_Page_Property_-_Menu`  
*	:ref:`Shared-Object-Properties_Object_Properties_-_Menu`  



