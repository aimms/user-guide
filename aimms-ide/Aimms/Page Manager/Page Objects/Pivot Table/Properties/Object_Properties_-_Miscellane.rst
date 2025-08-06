

.. _Pivot-Table_Object_Properties_-_Miscellane:


Misc
====

**Description** 

On the Misc. tab you can set a number of miscellaneous object properties (which are not captured under a specific property category or tab). These properties are applicable for most of the page objects.



**Include in Tab Sequence** 

The Tab Sequence is the user defined ordering of the page objects, that is used when changing the focus from one object to another, whenever the user presses the <Tab> or <Shift-Tab> keys. Here you can specify whether a object should be included in this sequence. If you do not include an object in the tab sequence, the end-user cannot get to the object using the keyboard, but he can still use the mouse to select it. This property can also be changed via the command Tab Order in the Edit menu.



**Use (Shift-)Tab within Object** 

By default, the <Tab> and <Shift-Tab> keys are used to change the focus on a page from one object to another. In some objects it may be more intuitive to use these keys to browse within the object itself.



**Keys for Leaving the Object** 

In most objects, the <Enter>, <Up>, <Down> and (optionally) the <Tab> key are used to browse through the data in the object. If the user cannot browse any further within the object (for example when he reaches the bottom of a table, while pressing the <Down> key), you can specify whether pressing any of these keys again will move the focus to the next object on the page.



**Tag Name** 

Via the tag name, you can enter a (unique) identification name for an object. You can use this name if you want to refer to a specific object (for example in the function PageSetFocus or PageSetCursor).



**Help Topic** 

You can enter a quoted string or a scalar string parameter in the help topic box. Help is activated when the user uses Context Help on the page object. Depending on the type of file that has been specified as the Application help file, the Help Topic needs to correspond to a k-keyword in a Windows Help file, a keyword in a compiled HTML Help file, or a named destination in a PDF Help file. AIMMS does not check whether the entered Help Topic exists in the Application Help file, so you have to ensure that yourself.



**Printing Occurrence** 

The property Printing Occurrence is only applicable if the object is placed on a so-called Print Page (i.e. it must depend on a Print Template in the Template Manager).

When printing a page it can occur that certain objects on the page contain more information than can fit on one sheet of paper (for example, a very long table). In that case, you can instruct AIMMS to spread the contents of this object over multiple output pages (sheets). For every output page that is created during the printing, AIMMS tries to print any other object as well. Via the Printing Occurrence property, you can select a condition to print or not print an object on an output page. These conditions are:

*	Every Page.
*	Spread over Pages.
*	Only on First Page.
*	Not on First Page.
*	Only on Last Page.
*	Not on Last Page.
*	Do Not Print.




**Note** 

*	Button and Selection objects cannot be printed on an output page. You can, however, place these objects on a Print Page, and use them for navigational purposes.




**Learn more about** 

*	:ref:`Miscellaneous_Help_Files_for_AIMMS_Projects` 
*	:ref:`Template-Manager_Print_Templates_Introduction` 
*	:ref:`Page-Manager_Tags`  



