

.. _Document-Viewer_Document_viewer_Properties_Con:


Contents
========

**Description** 

This tab contains the properties that let you control what is shown in the document viewer object.



**Document URL** 

This property specifies what document/file you want to display in the document viewer. A lot of file types can be displayed. You can also specify a web page URL.



**Update URL string parameter** 

With this property, you can specify whether string parameters containing the document URL should be updated or not. 
For example, if you have specified a string parameter for the "Document URL" property, and 
this string parameter contains the value "https://www.aimms.com", then it still contains this value 
after displaying this particular web site if the "Update URL string parameter" property has value 0 (the default). 
If this property is set to 1, the string parameter contains "https://www.aimms.com/" after displaying the web site. 
Also, when following links from a web site, the string parameter will be updated to the new site(s) visited if 
this property is set to 1, but will remain the initial value if set to 0.



**Allow Navigation** 

If you set this property to 'No' and the document viewer is displaying a web page, clicking on any link inside the web page will not have any effect.



**Enable Browser Context Menu** 

If the document viewer is displaying a web page, then when you right-click in the object, a browser defined context menu is shown. If you don't want this menu to be available to your end-users, you should set the value of this property to 'No'.



