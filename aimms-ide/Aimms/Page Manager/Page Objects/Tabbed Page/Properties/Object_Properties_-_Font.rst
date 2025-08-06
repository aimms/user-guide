.. |img_def_default_property_bmp| image:: images/default_property.bmp


.. _Tabbed-Page_Object_Properties_-_Font:


Font
====

**Description** 

AIMMS manages a font list that contains all the types of fonts that are used in the interface. If you select a font for an object, then the object only keeps a reference to an element in the font list. This means that, if you modify a font in the font list, then this change is automatically propagated to all the objects using that specific font. 

In the Font tab of an object you can select the font to be used for the object, but it also offers you the tools to modify and manage the font list.



**Note** 

Every newly created object initially uses the default font. You can set this default font in the Font tab, using the small menu that appears when you press the |img_def_default_property_bmp| button. This menu contains two commands:

*	Set as Default: this will set the currently selected font as the default font (that is used when a new object is created).
*	Reset to Default: this will select the font that is currently used as default font.




**Tips & Tricks** 

*	Name fonts after their intended use in the end-user interface, rather than using names that reflect, for instance, the font name and size used. By doing so, you will prevent that a font that you created for a particular purpose is used in other places in the interface as well. The latter may make it very hard to change the font's appearance without creating all sorts of difficulties elsewhere in the interface. For example, when a font is called 'Button font' it is very likely that this font will only be used for buttons, and not in tables as well. Such a clue of intended use is not present when the font is named e.g. 'Arial, 8pt'. In the latter case, you will, without doubt, find yourself having to go through the entire interface at some point in time to verify the (unwanted) effects of a change of font. Thus, you can easily improve the maintainability of your project, by choosing appropriate names.




**How to …** 

*	:ref:`Fonts_Editing_a_Font` 
*	:ref:`Fonts_Introducing_a_New_Font` 
*	:ref:`Fonts_Deleting_a_Font` 
*	:ref:`Fonts_Renaming_a_Font` 



