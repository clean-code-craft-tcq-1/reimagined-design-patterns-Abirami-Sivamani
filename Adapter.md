# Adapter Design Pattern

Adapter is a structural design pattern, that works as a brige between two incompatible interfaces.
Adapter pattern converts the interface of one object so that another object can understand it. 

**When to Use?**
1. When you want to use some existing class, but its interface isn't compatible with the rest of the code
2. When you want to reuse existing subclasses that lack some common functionality that can't be added to the superclass

**Real time examples**

1. Let us consider a card reader, which act as an adapter between memory card and laptop. we can plugin memory card into the card reader and card
reader into the laptop. so that memory card can be read through laptop
2. Let us consider a mobile charger plug and power supply socket has different design. hence mobile charge plug won't fit into the socket. In this case,
we can use power plug adapter that has the socket(as mobile charger required) and plug(as socket required) format. 

**Advantages**

1. Single Responsibility Principle : We can separate the conversion code from the primary domain/business logic code
2. Open/Closed Principle : We can use n number of adapters without making any changes on the existing client code

**Disadvantages**
1. Sometimes it will increase the complexity of the code, as number of interfaces and classes grows.
