

.. _Page-Manager_Page_Property_General:


General
=======

**Description** 

On the General tab of the page properties dialog box you can set the following properties:



**Title** 

The title of a page is the text that appears in the caption of the page window and in the navigation objects / menus. If you do not specify an explicit title, then the page name is used, which is the unique name of a page, as it appears in the Page Manager and Template Manager. The title of a page is only used for display purposes. If you need to refer to a page (for example in the PageOpen procedure), then you should always use the page name. The specified title can be a static string or a reference to a scalar string parameter.



**Behaves as Dialog** 

If you specify this style for a page, then the page will be opened as a dialog box. This means that the page gets the exclusive focus and the end-user cannot switch to other pages or use any of the menus without closing the dialog page first. You should use this style in situations where you want to force your end-user to give certain inputs. Usually, a dialog page is equipped with an OK and Cancel button.



The style 'Behaves as Dialog' is ignored when the page is opened from the Page Manager, the Template Manager or via the File – Open – Page menu. To open the page as dialog box, you must open it either via a button action or via a call to any of the PageOpen procedures.



**Save Last Position** 

This property is only valid if 'Behaves as Dialog' is enabled. If you enable this option, AIMMS will reposition a dialog at the same position (and with the same size) as the last time the dialog was opened and closed. So if a user moves or resizes the dialog page, a next time it is opened, this new position will be remembered.



**Always Docked** 

By default a page appears in the Document Area of the IDE (see also :ref:`Page-Manager_Making_a_Page_dockable`). If you enable the style 'Always Docked', then a page will always open in docked mode, and a user cannot put it back to the Document Area. If you check this option in the property dialog box while the page is not yet docked, then upon Apply (or OK), the page will become docked automatically.



**Allow User Dockable** 

If it is useful to have a certain page being docked based upon the end-user's choice. You can set the style to 'Allow User Dockable'. After applying this style, the menu command **View - Show Docked**  is enabled, and can be used to switch between docked and non-docked state. This menu command is also available when you right-click in the title area of the page. Once a page is in Docked mode, you can drag it to any position within the main AIMMS window, or to a 'floating' position anywhere on your screen. 



**Include in Saved Layout** 

This property is only valid if either 'Always Docked' or 'Allow User Dockable' is enabled. If checked for a page, then each time the current layout of docking windows is saved, the page is included in this saved layout. This implies that, if such a saved layout is restored (either at project startup, or via the menu command **Windows - Layout - Reset**), the page is automatically (re-)opened as well. See also: :ref:`Miscellaneous_Saving_and_Restoring_Layouts` .



**Close Page when Inactive** 

You should always try not to keep too many pages open at one time. One way of achieving this, is by selecting this style for your pages. As soon as another page gets the focus, all other pages that have this style will be closed automatically.



**Page (Edit) Size** 

The size of a page is only relevant in any of the following situations:


*   The page 'Behaves as Dialog', in which case the specified size is used as the (initial) size of the dialog box.
*   The page is used as the inner page of an :ref:`Indexed-Page_Indexed_Page_Object_-_Introduc`  and the size of the inner page is not defined by the Indexed Page object itself.
*   The page is resizable, in which case the specified size will be used whenever you put the page back in Edit Mode.



**Inherited from Template** 

By default this property is enabled and implies that the size is inherited from the template that is the parent of the active page or template in the Template Tree. If you are in one of the situations described above, and the current page or template does not have a parent template, then it is useful to disable this property and specify the **Width** and **Height**  explicitly. Please note that if a parent template exists and the parent template is resizable, then it is not possible to disable this option.



**Specific Width & Height** 

If you set the specific width and height, the page or template no longer inherits its size from a parent template. 



**NOTE:** If you change the size of a page or template that is resizable, the resizing algorithm itself will be used to reposition all page objects correctly. In other templates and pages that are descendants of the current template (and thus inherit the changed size), this repositioning of the page objects must also take place. If this applies for the current template, then a dialog box will pop-up in which you can confirm that all these depending templates and pages should be modified as well.





**Help Topic** 

You can enter a quoted string or a scalar string parameter in the help topic box. Help is activated when the user uses Context Help on that page. Depending on the type of file that has been specified as the Application help file, the Help Topic needs to correspond to a k-keyword in a Windows Help file, a keyword in a compiled HTML Help file, or a named destination in a PDF Help file. Make sure that the Help Topic exists in the Application help file. 



**Hidden** 

You can enter a scalar model identifier or a value that controls the hidden status of the page or template. If the corresponding value is not equal to 0, the page is hidden. The hidden status has effect in four different areas:

*	Navigation Object: The page is not visible.
*	Navigation Menu: The page is hidden.
*	Button Action Goto: The page is skipped.
*	Templates: Hidden templates are ignored when a page is opened that depends on this template.




Only while opening a page, the hidden status is considered. This means that changing the 'hidden' identifier on a page has no direct effect on the page.








**Learn more about** 

*	:ref:`option-AIMMS-application_help_file`  



