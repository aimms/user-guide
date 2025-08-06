

.. _Button_Action_-_Goto_Page_-_Previous1:


Goto Page - Previous in Tree Walk
=================================

To add an action that opens the previous page in the tree walk:

1.	While in Edit Mode, open the Properties dialog box of the Object you wish to assign the action to.

2.	Change to the Action tab.

3.	Select the Goto Page action from the Select Action to Add list and click Add.

The Goto Page window appears on the right hand side of the tab

4.	Select Previous in Tree Walk in the selection box.

5.	Select what you want to happen if there is no previous page in the tree walk. You can choose to 'Go Nowhere', or 'Use a cyclic sequence'.

6.	Specify the Number of Ancestor Levels. The number of ancestor levels from the active page specifies the root of the subtree that should be considered for the tree walk.

7.	Specify the Number of Descendant Levels. The number of descendant levels from the active page specifies the depth of the subtree that should be considered for the tree walk.

8.	Select whether you want to 'Combine with following go to page action'. If you select this and there is a following page action, AIMMS will combine the two and will use the result of this go to page action as the reference page for the next go to page action, without actually opening this page.

9.	Click Ok.





