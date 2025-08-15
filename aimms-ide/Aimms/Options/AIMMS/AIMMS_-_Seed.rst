

.. _Options_AIMMS_-_Seed:


Seed
====



**Type**:	Integer	

**Range**:	{1..:ref:`Miscellaneous_Maxint`  }	

**Default**:	3141	



With this option you can set the seed of the random number generators for all distributions. By setting the seed to a specific number you can guarantee that your model results are reproducible. By setting the seed using for example the number of seconds or even ticks of the current date (using CurrentToMoment), you can get results that are not reproducible.



**Learn more about** 

*	:any:`CurrentToMoment`



