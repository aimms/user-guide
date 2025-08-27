

.. _option-AIMMS-use_empty_toolbar_instead_of_none:


Use Empty Toolbar instead of None
=================================



:Type:	Selection	
:Range:	One of the values listed below 	
:Default:	Never



Possible values are:



    *	Never
    *	Only in develop mode
    *	Always




For pages and some of the other windows in AIMMS, you can specify that you don't want a toolbar to appear at the top of the AIMMS window. If you mix this with windows that do have a toolbar, switching between these windows has the effect that the windows move up and down because of the appearing or disappearing toolbar.





If you don't want this (annoying) moving of the windows, you can use this option to override the meaning of 'no toolbar'. If you set this option to 'Always' then instead of no toolbar, you get an empty toolbar. If you set this option to 'Only in develop mode' then you only get this empty toolbar when you are running AIMMS in developer mode and in the end-user version of the project, no toolbar will appear. 

