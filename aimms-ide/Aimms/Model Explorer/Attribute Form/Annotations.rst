

.. _Model-Explorer_Annotations:


Annotations
===========

**Description** 



Some libraries in AIMMS (such as WebUI and CDM) define Annotations that can be attached to certain identifier types in your model. What these annotations do depends on the library.

When there is a relevant annotation available for a certain identifier, the Attribute Form shows the 'Add Annotation' wizard. Via this wizard you can select the annotation that you want to specify.



Please note that annotations can be inherited from the parent nodes in the Model tree. If that is the case, you will see the inherited value and this value is not directly editable.



For each specified annotation the wizard button shows a popup menu with a selection of the following commands:




*   **Override Inherited Value**  This means that the current value of the annotation is inherited from one of its parent nodes in the model tree. Selecting this command breaks this inheritance and allows you to specify a new value for the annotation.
*   **Wizard...**  Some types of annotations have a specific wizard dialog box to help you in specifying the correct value.
*   **Remove**  This clears the currently specified annotation value. If the parent node has a value for this annotation, it will be inherited.
*   **Help** This shows a short text (provided by the library that defines the annotation) explaining what the annotation is used for.



