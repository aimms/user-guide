

.. _option-AIMMS-standard_reports_empty_columns:


Standard Reports Empty Columns
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No Listing	



This option controls whether or not a listing of the empty columns generated is made. Possible values are:



    *	No Listing
    *	Only Symbolic Variables
    *	All Individual Variables




This option controls whether or not a listing of the empty columns generated is made. Possible values are:


When the value of this option is Only Symbolic Variables the output will look something like:








The generated mathematical program "myNetw" contains 6961 empty columns:


Flow(i,j) : 961;


PipeBuilt(i,j,k): 6000





When the otpion is set to All Individual variables, the output will look something like





The generated mathematical program "myNetw" contains 6961 empty columns:


Flow(a,b)


Flow(a,c)





and so on.

