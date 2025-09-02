

.. _option-AIMMS-progress_generation:


Progress Generation
===================



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	1	



This option controls progress reports during the generation of the matrix. If the :ref:`aimmshelp12-progress_window` is open,
it will display information about how many rows, columns and nonzero matrix elements are generated. Possible values are:

    0:	Do not report progress.	

    *n*:	Report progress after the generation of every *n* constraint blocks.	

