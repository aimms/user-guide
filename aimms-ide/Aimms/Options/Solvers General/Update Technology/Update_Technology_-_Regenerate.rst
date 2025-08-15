

.. _Options_Update_Technology_-_Regenerate:


Regenerate Threshold
====================



:Type:	Integer	
:Range:	{0..100}	
:Default:	25	



This threshold determines when AIMMS will regenerate the model from scratch or will update the previous setting of the model. If the number of terms to be regenerated for the update is less than Regenerate Threshold percent of the total number of terms, then AIMMS' update technology will be applied. Hence, a value of 0 corresponds to a setting, in which the matrix is always regenerated from scratch, whereas a value of 100 always forces AIMMS to update the matrix.



