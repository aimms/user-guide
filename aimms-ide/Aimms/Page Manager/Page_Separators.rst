

.. _Page-Manager_Page_Separators:


Page Separators
===============

**Description** 

A page separator divides a set of pages with the same parent page into two separate cyclic, double-linked lists of pages. The first cyclic, double linked list can be entered by opening the child page of the parent page. To open a page in one of the other lists, you should open it explicitly, either via a PageOpen command or via a Page Link action at a button or menu. Once a page in this other list is opened, the default navigation actions can be used to open related pages.



**Tips & Tricks** 

*	To exclude maintenance pages (i.e. pages that are only used during the development of an application) from an end-user application without explicitly deleting these pages, group the maintenance pages and insert a page separator before the first maintenance page.



