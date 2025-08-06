.. |img_def_Properties_button_bmp| image:: images/Properties_button.bmp


.. _Menu-Builder_Specifying_a_Shortcut_Key:


Specify a Shortcut Key
======================

**Description** 

For each menu item contained in a menubar you can defined a shortcut (or accelerator) key. Usually, this key is defined as one of the function keys on your keyboard, or key combinations using the ``<Ctrl>``  or ``<Alt>``  key. If a menu item has a shortcut key, then the specific key(-combination) is displayed in the menu. The shortcut key of a menu item can be used to directly execute the command, without explicitly accessing the menu.

To specify a shortcut key for a menu item node:

1.	Open the Menu Builder.

2.	In the tree, select the menu item node.

3.	From the Edit menu, select Properties |img_def_Properties_button_bmp|.

4.	Go to the Shortcut Key field.

5.	Type the key combination you want to use as shortcut.

6.	Click Ok.



**Note** 

*	Shortcut keys only work for menu items, not for items in a toolbar.
*	Some key combinations are commonly used in many windows applications, and most people are very familiar with them. For example: in most applications ``<Ctrl-C>`` , ``<Ctrl-P>`` , and ``<Ctrl-V>``  are used for the cut, copy and paste commands, and <F1> is used to access the help facilities. In the Menu Builder, you can redefine all these key combinations, but you should realize that this may confuse your end-users.
*	The Menu Builder allows you to specify single-character shortcuts like ``<A>`` , ``<B>`` , etc. However, you should be careful using these type of shortcuts, because the specific key can then no longer be used for regular editing. For example, if you define a shortcut ``<H>``  for some menu item, the user can not simply type the string "Hello" anywhere within that page.
*	In addition to the explicitly defined shortcuts, you can access every menu using an ``<Alt>``  key combination. If you press the ``<Alt>``  in combination with the first character (or an underlined character) in a menu title, the menu will be opened, and you can further select the specific command to be executed. For each menu in the menu bar, you can decide which character should be used for this ``<Alt>``  key stroke.




**Learn more about** 

*	:ref:`Menu-Builder_Menu_Node_Property_-_Descripti`  



