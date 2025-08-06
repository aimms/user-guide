

.. _Menu-Builder_Menu_node_properties_control:


Control
=======

**Description** 

On the Control tab of the properties dialog box in the Menu Builder, you can specify some additional options that control the appearance of a specific item in a menu or toolbar.



**Disable** 

With this option you can disable a popup menu or menu item. Disabled popup menus and menu items are grayed-out and cannot be accessed. You can specify that the menu or item is disabled permanently, but normally you will use a scalar parameter to indicate the disabled status, so that you can change the status from within your model. A nonzero value of the parameter corresponds to a disabled status.



**Check** 

If you specify a scalar parameter for this option, then the corresponding menu item will get a check mark if this parameter is not equal to 0. Similarly, if the user selects the menu command, the value of this parameter will toggle from 0 to 1 (or vice versa). If there are any further actions defined for the menu item, then these actions will be executed after the value of this parameter is changed. If the menu item is used as a toolbar button, the checked state of the item is represented by a button that is 'pressed-in'.



**Hide** 

In addition to disabling a part of your menu, you can choose to completely hide it from the end-user. Similar as for the Disable option, you can set the hide status using a scalar parameter.



**GUI Name** 

If you specify this option, then in the resulting menus this name will be used instead of the default name that is specified on the Description tab. In the Menu Tree however, you will always see the default name of the node. This option is especially useful to support multiple languages within your menus: you can specify the GUI Name via a string parameter, and thus let the name depend on your current model data.



**Window list** 

If set for a specific popup menu, the popup menu is extended with a numbered list of all currently open windows. The currently active window is indicated with a check mark.



**Tips & tricks** 

*	When using model parameters for the disable, hide and GUI-name properties, menus can be customized (disables, hidden or renamed) depending on, for example, the user.




**Learn more about** 

*	:ref:`Miscellaneous_Localization`  



