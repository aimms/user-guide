

.. _Picture_Bitmap_Object_Properties_-_Bit:


Picture
=======

**Description** 

The Picture Property Tab contains the specific properties that are available for the picture object. You can adjust the following properties here:



**File Name/Identifier** 

To draw a picture on a page, Aimms always needs an image file (supported files are: BMP, EMF, Exif, GIF, ICON, JPEG, JPG, PNG, TIFF, and WMF). This file should either be available on your disk, or should be imported in your project file as a Project User File. Besides specifying the location of the filename directly, you can also specify a string parameter that contains a reference to a file name.



**Size/Location** 

This property defines how it is displayed if the rectangular area does not have the same size as the image itself and how the image is located. You can choose between three size modes:

*	Actual Image Size. The image is displayed using the size that is stored in the image file; if the picture is too large, then the remaining part is cut-off, if the picture is too small, then the remaining part of the rectangle is not filled.
*	Stretch/Shrink to Rectangle. The picture will be stretched or shrunken (vertically and horizontally) so that it exactly fills the specified rectangle.
*	Fill with Multiple Images. If the picture is too small to fit in the rectangle (vertically or horizontally or both), then the rectangle is filled with as many copies of the pictures as possible.

For Actual Image Size and Stretch/Shrink to Rectangle combined with Keep Original Ratio, you can choose to center the image file in the rectangle by checking Centered.


When Stretch/Shrink to Rectangle is chosen, you can keep the original image ratio (height vs. width) by checking Keep Original Ratio. The remaining part of the rectangle is not filled.





**Colors** 


This property defines the colors of the image in the picture object. You can change the intensity of the colors by moving the **Intensity**  slider more to Light or Dark. To make the image transparent, you can check **Use Left-Bottom Pixel as Transparent Color** . This checkbox is only meant for images that do not already contain transparency itself (e.g. not for .ico files).










