.. _CPOPT_Parallel_-_Number_of_workers:


Number of workers
=================



**Type** :	Integer	

**Range** :	{-1..2100000000}	

**Default** :	-1	



This option sets the number of workers to run in parallel to solve your model. If the number of workers is set to n (with n greater than one), then CP Optimizer will create n workers, each in their own thread, that will work together to solve the problem. The emphasis of these workers is to find better feasible solutions and not to speed up the proof of optimality.



The default value of -1 amounts to using as many workers as there are CPU cores available on the machine.



Note that the memory required by CP Optimizer grows roughly linearly as the number of workers is increased. If you are solving a very large model on a multi-core processor and memory usage is an issue, it is advisable to specify a reduced number of workers, or even one worker, rather than use the default value.



