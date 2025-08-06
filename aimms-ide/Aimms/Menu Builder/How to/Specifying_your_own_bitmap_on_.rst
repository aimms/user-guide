

.. _Menu-Builder_Specifying_your_own_bitmap_on_:


Specify Your Own Bitmap on a Tool Bar Button
============================================

**Description** 

In the Properties dialog box of a menu item, you can select the bitmap image that should appear on a toolbar button. AIMMS has a number of built-in images from which you can select, but you can also add your own set of images.

All these images must be presented to the Menu Builder in one bitmap file. The individual images in this file must be such, that each single image should has a size of 16x16 pixels, and they are positioned next to each other (in one row). The total bitmap is thus 16 pixels in height, and a multiple of 16 pixels in width.



To add your own bitmap file with toolbar button images to the Menu Builder:

1.	Open the Menu Builder.

2.	From the Edit menu, select User Bitmapfile.

In the dialog box:

3.	Specify the name of the bitmap file.

4.	Press OK.

After having specified a user bitmap file, the user-defined images are added to the image list on the Description tab of the Properties dialog box.



**Tips & Tricks** 

*	Instead of using a bitmap file from disk, add the bitmap file to the User Project File and reference that file.
*	In the subfolder '``Templates\Bitmaps`` ' of the AIMMS installation folder, you find a bitmap file '``User Toolbar Bitmaps.bmp`` ' that can serve as a template to create your own user bitmaps.



