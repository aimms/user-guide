

.. _Navigation_Navigation_Object_Properties_-:


Navigation
==========

**Description** 

In the navigation tab, you can adjust the following properties:



**Style** 

From this drop down menu, you can select the display style for the navigation object.

*	Text Button	buttons with as text the page titles
*	Button + Text 	small buttons with next to them the page titles
*	Text		only the page titles
*	Tree		a tree similar to the page manager tree
*	Expanded Tree	similar to tree, but totally expanded




**Reference Page** 


The Navigation object displays the pages from a specific part of the Page Manager tree. Which part is displayed first depends on the Reference Page, from this page you can then specify how many levels of child pages (generations) and how many levels of parent pages (ancestors) you want to see.


You can specify the reference page relative to the page on which the object is placed, or you can simply pick a specific page from the Page Manager tree.





**Layout** 


Depending on the chosen Style you can specify some extra layout properties. You can choose to have the text centered horizontally (instead of right-aligned), and you can choose to spread all entries evenly vertically. Spread evenly only has effect when also a maximum number of items is selected and the number of items that are actually shown is smaller than this maximum. In that case the items are evenly spread vertically over the total size of the navigation object. As an alternative for spread evenly you can also specify a number for the Item Spacing (in pixels). For the Text Button and Text style you can also select to have the button horizontally instead of vertically.





**Open Page upon Single Mouse Click** 


This option specifies whether in Tree or Expanded Tree style a page should be opened upon single mouse click instead of double mouse click. 





**Number of Generations from Reference** 


This number indicates how many generations from the reference page should be shown in the navigation object. A value of 1 a means that the child pages of the reference page are shown, a value of 2 shows also the children of the child pages, etc … 


A value of 0 does not show any child pages.





**Number of Ancestors including Reference** 


This number indicates how many ancestors from the reference page should be shown in the navigation object. A value of 1 shows only the reference page itself, a value of 2 also shows the parent page, etc…


A value of 0 does not show the reference page or any of its ancestors.





**Include Hidden Pages as Disabled** 


If this property is turned on, hidden pages will be shown disabled. You will not be able to jump to the hidden pages ( but you can jump to child pages of these pages). If this property is turned off, hidden pages and children of hidden pages will not be shown in the navigation tree.





Changes in the hidden status via a parameter will only be effective when a page is reopened.





**Exclude the Containing Page Itself** 


If this property is turned on, the page that contains the navigation object will not be part ot the buttons on the navigation object.





**Note** 

*	On a template page, if you select the This Page as the reference page, then this page does not refer to the template, but to the page that is created using that template. If you open the template itself, the navigation object will not show any page references (because a template is not part of the Page Manager tree).






