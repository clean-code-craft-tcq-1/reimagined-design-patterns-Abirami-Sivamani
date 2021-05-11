# State Design Pattern

State is a behavioral design pattern that allows the object to change its behavior based on the object state. 
In state pattern, we can create objects which represent various states and a context object whose behavior varies as its state changes.

**Example**
Let us assume a media player, which has a button to start and stop playing the media. If Player is in on state, clicking on the button will stop the player.
If player is in off state, clicking on the same button will start the player. In this case, same button will act differently based on the player state(on/off).

**when to use?**

1. When object behaves differently based on the state, and if object has more number of states and requires frequent changes on the state specific code.
2. When class has multiple conditionals that will change based on the state of the objects.
3. When we have lot of duplicate code across similar states.

**Advantage**

1. Single Responsibility Priniciple - Separating into multiple class based on the states available and segregating the static specific behavior to the respective state class
2. Open/Closed Principle - Can add new state class without making any changes on the existing state classes or the context class.
3. Reduces the complexity by eliminating the state conditional statements

**Disadvantage**
1. Won't be useful if class has few states or it has the same behavior over multiple states
