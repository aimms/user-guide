

.. _Options_Compilation_JIT_Body_compilation:


JIT Body Compilation
====================



:Type:	Selection	
:Range:	On or Off	
:Default:	Off	



With this option you can enable the feature "Just-in-Time (JIT) Body Compilation". 

When enabled, at startup of the app, the compilation of the model will skip all the Body attributes of procedure and functions. 

Only when the procedure or function is to be executed, the body will be compiled just at that moment.



This feature is especially useful for end-user sessions, where you want to minimize the waiting time until the application is completely initialized and ready for input. That is: the time between starting the app and the moment the first page is presented. 



Another benefit may be in AIMMS PRO (solver) sessions where the server starts the app to, in some situations, only run one single procedure.



In a develop session, the effect of the JIT compilation is less. It will reduce startup time, but as soon as you start making model changes and/or press F5 (Compile All), all body attributes will be compiled. Please note that this also helps in making sure that the model that you develop does not contain compilation errors when you create an aimmspack for it.



When a procedure body contains a syntax error, the JIT Compilation will hit a compilation error when the procedure is about to be run. This error will popup as an execution error. As with any other error you can handle this error via the error handling mechanisms in AIMMS. By default, the error will stop further execution and popup in the error window. 







