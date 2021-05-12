# Decorator Design Pattern

Decorator is a structural design pattern that allows us to add new behaviors to the object dynamically at the runtime by placing them inside special wrapper objects.
This pattern creates a decorator class which wraps the original class and provides additional features keeping the class methods signature intact.

**When to Use?**

1. When you need to add extra functionality to the objects at the runtime without breaking the code that uses these objects.
2. When its not possible to extend an object's behavior using inheritance.

**Example**

Let us consider a simple example of pizza. Pizza interface has GetName(), GetCost(), GetDescription() methods
Margheritta, Paneer, Mushroom Pizza class implements the Pizza interface. 
Toping is the decorator class, which implements the same pizza interface.
We have number of topings for the pizza. we can add those extra behaviors at the runtime to the original object of pizza.

**Advantages**
1. We can extend object's behavior without making a new subclass
2. We can add/ remove the features from an object at runtime
3. We can combine several behaviors by wrapping an object into multiple decorators.
4. Single Responsibility Principle

**Disadvantages**
1. Its hard to remove specific wrapper from the wrappers stack
2. Its hard to implement a decorator in such a way that its behavior doesn't depend on the order in the stack
