<h1>SENG330</h1>

<h3>Lecture 1</h3>

Principles

- Experts prefer solutions they know work
- Experts move among levels of abstration
- Experts make tradeoffs
- Experts use notations (UML) as a lens and not a straightjacket
- Experts design through the creation of software

<h6>Definition of Software Design</h6>
Software design concerns determining the abstraction structure of the intended software

To do:
Get Eclipse Workspace set up

<h3>Lecture 2</h3>

Encapsulation

Encapsulation - Information Hiding

What to show, and what to keep internally

Benefits:

- security
- simplicity
	- decompose
- information hiding

1. A good abstraction maps to domain & solves a solution in the real world
2. Encapsulation is the other property of a good abstraction. Want to keep an abstraction simple to avoid the complex details

Global variables and the goto statement (ex// exceptions like null pointer) violate the principles of abstraction.
With global vars any other aspect of the system could inadvertently change that value.



Team
<ul>
<li>Chief devs</li>
<li>Devs</li>
<li>Testers</li>
</ul>

Customers (don't want to expose everything to customers)

Classes

- interfaces that have implementations
- outside users shouldn't be able to see the implementation

Build tools take care of figuring out where everything should be
ex//
- maven
- gradle (one we're using)

$ gradle build
(runs checkstyle and assembles everything)

Bookstore Inventory
- common abstractions

In OOP, nouns are objects and verbs are functions

Leaky abstraction
- an abstraction that requires knowledge of an underlying complexity to be able to know how to use it

Monday 2-3pm ECS561 - Office hours

<h2>Lecture 4</h2>
1. Make fields private
2. Not every field needs to be accessed
3. Avoid method that sets / returns values
4. Final makes stuff immutable
immutable 
	- parallelizable
	- predictable
	- security

<h2>Lecture 5</h2>
Private - Class or object scope 
Stuff insdie of a method - local scope
Everything that has global scope would be a part of the interface
Class becomes an object when it becomes instanced, ie using the new keyword

Interfaces are like contracts. 
Anything that implements this interface must implement these methods.

public class Joker extends Card implements Comparator

<h6>Polymorphism</h6>
- Rough shape
- I don't know the particular details, but it has to do this and this other thing

<h2>Design Patterns</h2>
- Name 
- Context
- Solution
- Consequences / Tradeoffs

ex//
- Factory method
- Iterator
- 