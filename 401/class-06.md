# Read Calss - 06 : Authentication
## Explain what a “Singleton” is (in Computer Science terms)
A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

## Explain how the Singleton pattern can be used with Node modules, specifically with classes
Use the Singleton pattern when a class in your program should have just a single instance available to all clients; for example, a single database object shared by different parts of the program. The Singleton pattern disables all other means of creating objects of a class except for the special creation method.
> This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.

## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
In Express, you can set up middleware to be “global” middleware; meaning it will be called for every incoming request. it's like for each middleware I'll create a class to be used all over the system.
