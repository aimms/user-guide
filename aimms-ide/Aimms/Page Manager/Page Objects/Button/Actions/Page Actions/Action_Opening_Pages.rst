

.. _Button_Action_Opening_Pages:


Opening Pages
=============

**Description** 

There are two different actions that open pages and can be added to the action list of a button, these are

*	Goto Page 
*	Linked Page(s)

The action Goto Page defines a dynamic link to another page, i.e. the page to be opened is taken from the tree structure in the Page Manager. The action Linked Page(s) defines static links to other pages, i.e. the name of the page to be opened is stored as part of the action.





With the action Linked Page(s) you can link to multiple pages. In that case you have three extra options for opening (one of) these pages:

*	All of the linked pages are opened.
*	The user gets a dialog box in which he can select the page(s) to be opened
*	One of the linked pages is opened depending upon an identifier value. A value of 1 will open the first linked page, a value of 2 will open the second linked pages, etc.




**Tips & Tricks** 

*	If you open another page via the button actions, it is better to also add the action for closing the current page. If you do not do this you may end up with a lot of pages that are still open and this may decrease the performance of your application, because AIMMS will constantly keep the data in all open pages up-to-date with the last changes. Another reason for not keeping too many pages open is that that pages may take too many of Windows' resources.
*	Instead of using the Close Page action, you can use the option Close when Inactive in the Properties dialog box of the page. This automatically closes the page if another page becomes active.




**How to add an action that …** 

*	:ref:`Button_Action_-_Goto_Page_-_Next_Page`  
*	:ref:`Button_Action_-_Goto_Page_-_Previous_`  
*	:ref:`Button_Action_-_Goto_Page_-_Parent_Pa`  
*	:ref:`Button_Action_-_Goto_Page_-_First_Chi`  
*	:ref:`Button_Action_-_Goto_Page_-_Nth_Child`  
*	:ref:`Button_Action_-_Goto_Page_-_Same_Chil`  
*	:ref:`Button_Action_-_Goto_Page_-_Same_Chi1`  
*	:ref:`Button_Action_-_Goto_Page_-_Next_in_T`  
*	:ref:`Button_Action_-_Goto_Page_-_Previous1`  
*	:ref:`Button_Action_Goto_Page_Previously_Vi`  
*	:ref:`Button_Action_Opening_a_Number_of_Pag`  




**How to…** 

*	:ref:`Button_Action_Add_a_Page_to_a_Linked_`  
*	:ref:`Button_Action_Remove_a_Page_from_a_Li`  
*	:ref:`Button_Action_Reorder_pages_in_a_Link`  




**Learn more about** 

*	:ref:`Page-Manager_Page_Manager_Introduction`  






