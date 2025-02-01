# Unexpected Behavior When Directly Modifying Instance Variables in Ruby
This example demonstrates a potential issue in Ruby when directly manipulating instance variables using `instance_variable_set`. While functional, this approach bypasses the class's defined methods, potentially leading to inconsistencies or breaking encapsulation if not used cautiously.  The solution illustrates safer alternatives involving accessor methods.

## Bug
The bug lies in directly modifying the `@value` instance variable instead of using a method to update the value. This breaks encapsulation and can lead to maintainability issues if the internal representation of the class changes.