# Prototype Design Pattern

Prototype design pattern is a creational design pattern that allows us to copy the existing objects without having any dependency with the concrete class.
The concept is to copy/duplicate an existing object rather than creating a new instance from scratch.

**Problem:**

  If we want to create an exact copy of the object. we have to create a new object of the same class. Then we have to go through all properties of the original object and 
have to copy the values to the new object. In this case, some of the class properties may be private and we can't access from outside. 
And its dependent on the original class to create a copy.

**Solution:**

  Prototype pattern allows to create a copy of the object through cloning process. It declares a common interface for all the objects which support cloning. 
This interface allows to clone an object without dependent on the original class object. The interface contains the clone method, which creates the current class object and copy all properties of the current object to new object.

**Advantage:**
1. Cloning objects without dependent on the original class and doesn't requries any complex logic for getting a copy object.
2. since we are cloning the object, we can copy the private properties values of the original class
3. Improves performance by reducing the time consuming

**Disadvantage:**
1. Every class of the prototype must implement the clone() method
2. Implementing clone() method is difficult  for the complex object that have circular references
