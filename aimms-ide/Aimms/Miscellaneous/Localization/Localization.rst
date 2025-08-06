

.. _Miscellaneous_Localization:


Localization
============

**Description** 

The localization features in AIMMS help you to setup your application for multiple languages. The basic idea behind the localization in AIMMS is that all text that appears in the graphical user interface is represented via string parameters in your model. During the initialization of the model, these string parameters can then be read from separate, language dependent input files.



For many of the string parameters that you (already) use in your application, you have to setup your own mechanism to define and store the text for other languages. However, for most of the single text strings that appear in your application (such as page titles, text in menus, descriptive text on pages, etc) the localization tool of AIMMS can help you. For these strings AIMMS can setup and maintain a special string parameter that holds all the strings for a specific language. During the development of your application, it is very easy to select strings from this parameter, or to create new entries in it, when needed.



**Learn more about** 

*	 Search for Localization (User's Guide)
*	:ref:`Miscellaneous_Localization_Setup`  
*	:ref:`Miscellaneous_Localization_Conversion`  
*	:ref:`Miscellaneous_Localization_Text_Wizard`  



