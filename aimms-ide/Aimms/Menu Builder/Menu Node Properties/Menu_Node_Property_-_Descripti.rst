

.. _Menu-Builder_Menu_Node_Property_-_Descripti:


Description
===========

**Description** 

On the Description tab of a node in the Menu Builder, you can specify some of the basic properties that define the specific menu component.



**Name** 

Name of the node in the Menu Tree. The name needs to be unique for menubars, toolbars and popup menus. Ampersand characters in names of popup menus and menu items will be displayed as underlined characters that can be used in combination with the ``<Alt>``  key to activate the corresponding menu. The name that you specify here does not necessarily have to be the name that is displayed in the end-user application. If your application is designed for multiple languages, then you can use a fixed name here, and specify an alternative (parameterized) name using the GUI Name property on the Control tab.



**Shortcut key** 

Provides the possibility to enter a shortcut key sequence that can be used as quick way to activate the corresponding menu. The shortcut key is specified by simply pressing the desired combination of keys on your keyboard. A description of the shortcut key as recorded will then be shown in the shortcut key edit box. The shortcut key is only used for menu items. By pressing the <``Shift`` > key in the edit box you can remove the shortcut key. Some shortcut keys used by windows, like <``Pause`` > and <``Ctrl`` >-<``Break`` > cannot be used as shortcut key for a menu item.



**Comment** 

Provides the possibility to add a descriptive line of text. This property is not used for any other purpose.



**Toolbar Bitmap** 

The bitmap image that you specify here, will be used if the menu item is (also) used as a button on a toolbar. You can select any image from the presented list. This list consists of the standard bitmap images of AIMMS plus the images of an optional User Bitmap File, that contains your own, application specific images.



**Default Item** 

This checkbox specifies if the menu item is the default menu item. The default menu item of a right mouse menu is executed when the user double-clicks the left mouse button in an object that uses this popup menu as its right mouse popup menu.



**How to …** 

*	:ref:`Menu-Builder_Specifying_your_own_bitmap_on_`  
*	:ref:`Menu-Builder_Specifying_a_Shortcut_Key`  
*	:ref:`Page-Manager_Double_Click_in_Page_Object`  



