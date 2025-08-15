.. _CPOPT_Search_-_Branch_limit:


Branch limit
============



**Type**:	Integer	

**Range**:	{0..2100000000}	

**Default**:	2100000000	



This option limits the number of branches that are made before terminating a search. A branch is a decision made at a choice point in the search, a typical node being made up of two branches, for example: x == value and x != value. A branch is only counted at the moment a decision is executed, not when the two branches of the choice point are decided. A branch is counted even if the decision leads to an inconsistency (failure).

