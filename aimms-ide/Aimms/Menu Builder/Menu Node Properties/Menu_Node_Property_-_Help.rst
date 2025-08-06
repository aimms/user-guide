

.. _Menu-Builder_Menu_Node_Property_-_Help:


Help
====

**Description** 

On the Help tab, you can specify several properties that may help the end-user to understand the meaning of a menu item.



**Help Topic** 

For each menu item, you can specify a help topic in your application help file that describes the specific command. From a page you can access this help topic in two ways:

*	From the Help menu, select What's This, and then select the menu command for which you want to get help, or
*	Highlight the menu command (without actually executing it), and then press the F1 key.

Depending on the type of file that has been specified as the Application help file, the Help Topic needs to correspond to a k-keyword in a Windows Help file, a keyword in a compiled HTML Help file, or a named destination in a PDF Help file. You must make sure that the Help Topic exists in the Application Help file. 





**Status line** 


A constant string or string valued model identifier that is displayed in the status line (at the bottom of the AIMMS window) when the end-user browses through the menus (without actually selecting a specific menu command).





**Tooltip** 


A constant string or string valued model identifier that pops up in a small yellow box, whenever you move the mouse pointer over a toolbar button (and keep it there for a small amount of time). 





**Note** 

*	Because AIMMS does not make an explicit distinction between toolbar buttons and menu items, both the Status Line and Tooltip properties can be specified for one specific item. However, the Status Line text is only applicable for menu items, and the Tooltip text only for toolbar buttons.



