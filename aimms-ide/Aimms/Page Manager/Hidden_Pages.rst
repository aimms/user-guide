.. |img_def_Properties_button_bmp| image:: images/Properties_button.bmp


.. _Page-Manager_Hidden_Pages:


Hidden Pages
============

**Description** 

Generally, the navigation sequence, which you setup in the Page Manager, is the same for all (types of) users. However, if you want to hide certain pages from some users, you can do so using the Hidden property of a page. If a page is currently hidden, then it is ignored in any of the standard page navigation components. For example, a navigation object (or menu) will not show an entry for a hidden page, and a Goto Page button action will skip a hidden page.

To hide a page in the navigation sequence:

1.	Open the page.

2.	Make sure the page is in edit mode, and that you have not selected any page object.

3.	From the Edit menu, select |img_def_Properties_button_bmp| Properties.

4.	Enter a scalar identifier for the Hidden option (if this identifier is not equal to 0, then the page will be hidden).

5.	Click OK.



**Note** 

*	A hidden page is only ignored in the standard page navigation. You can still open a hidden page using the Page Link button action or via a call to the PageOpen procedure.
*	A change in the hidden status of a page is not immediately propagated to a Navigation object that is currently visible in a page. Only after re-opening the page the entry in the Navigation objects becomes hidden or visible.




**Learn more about** 

*	:ref:`Page-Manager_Page_Properties`  



