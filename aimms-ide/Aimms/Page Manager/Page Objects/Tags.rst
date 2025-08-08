

.. _Page-Manager_Tags:


Tags
====

**Description** 

By default, objects on a page do not have a unique name, and thus it is difficult to reference a specific object. Via the Miscellaneous tab of the object Properties dialog box you can assign a tag name to an object. These tag names can be used in the following situations:

*	A call to the procedure PageSetFocus, or PageSetCursor.
*	When you want to redirect the standard page close to a specific button.




Additionally, AIMMS itself will use the specified tag names in the Tab Order dialog box.





If you do not specify a tag name AIMMS uses a default tag name containing the type of object ("button", "table", "curve", etc). As long as you only have one instance of a specific object type on your page, you can use this default tag as a unique reference.





**How to ...** 

*	:ref:`Page-Manager_Opening_the_Properties_Dialog_`  




**Learn more about** 

*	:ref:`Page-Manager_Tab_OrderTab_Sequence`  
*	:ref:`Page-Manager_Page_Property_-_Action`  
*	:any:`PageSetFocus`
*	:any:`PageSetCursor`



