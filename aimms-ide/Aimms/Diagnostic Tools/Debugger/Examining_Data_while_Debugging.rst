

.. _Diagnostic-Tools_Examining_Data_while_Debugging:


Examining Data while Debugging
==============================

**Description** 

Whenever you are in the debugger, AIMMS allows you to interactively examine the data associated with the identifiers in your model, and observe the effect of statements in your source code. The most straightforward method is by simply moving the mouse pointer over a reference to an identifier (or identifier slice) within the source code of your model. As a result, AIMMS will provide an overview of the data contained in that identifier (slice) in the form of a tooltip. 



If you need to examine the effect of a statement on the data of a particular identifier in more detail, you can simply open a Data Page, or observe the effect on ordinary end-user pages. Within a debugger session, AIMMS supports data pages for both global and local identifiers, thereby allowing you to examine the contents of local identifiers as well. After each step in the debugger, AIMMS will automatically update the data on any open end-user page.



**Note** 

*	Whether or not AIMMS shows tooltips for identifiers in the model tree or in the model text, is actually specified by two options that are located in the section Project – Tooltips of the Project Options dialog box. Initially, these two options have the value 'Only during debugging'.




**How to ...** 

*	:ref:`Page-Manager_Data_Page`  




**Learn more about** 

*	:ref:`option-AIMMS-identifiers_in_model_tree`  
*	:ref:`option-AIMMS-identifiers_in_model_text`  






