.. _CONOPT_Stop_Criteria_-_Accuracy_One_Dim_Search:

Accuracy One Dimensional Search
===============================



:Type:	Floating point number	
:Range:	[0.05,0.8]	
:Default:	0.2	



This option determines the relative accuracy of the one-dimensional search. The one-dimensional search is stopped if the expected further decrease in objective estimated from a quadratic approximation is less than the value of this option times the decrease obtained so far. The default value is 0.2. A smaller value will result in more accurate but more expensive line searches and this may result in an overall decrease in the number of iterations. Values above 0.7 or below 0.1 should not be used.



