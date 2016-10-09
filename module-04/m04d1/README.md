# Module 04: Day 1 - Objects &amp; Classes 
Classes and Objects lay at the heart of Java.  Until this point we have had to cover the foundation of programming (variables, conditionals, simple I/O and loops) as well as some core skills (getting a program to run and watching it execute so as to debug).  Now that we have that foundation laid, we can turn our attention to a core element of the Java: Object Orientation (aka "OO").  In the late 80s, this was the &quot;Promised Land&quot; (that&apos;s a biblical metaphor for *the future of programming*).  

With OO, a new realm of programming opened up.  It became easier to deliver more complex problems as they could be broken down into simpler units.  OO removed complexity and ensured a common understanding leading to standards that in turn has allowed us to develop bigger (and distributed) systems.

In this segment we'll first cover theory (and how it arose); then go through a series of videos (by Bana) that show how Java provides these features.

## Materials & Resources

| Link | Comment |
|:---- |:------- |
|https://www.youtube.com/watch?v=pBlH24tFRQk |The origins of OO.|
|https://www.youtube.com/watch?v=eKC04ztp09o |What are objects (JCode.03)|
|https://www.youtube.com/watch?v=X8D2FVAfNtI |What is a class (JCode.04)|
|https://www.youtube.com/watch?v=UDVVPUqjsRg |What is a field in a class (JCode.05)|
|https://www.youtube.com/watch?v=chWtlHxYS8Y |Methods (JCode.06)|
|https://www.youtube.com/watch?v=Lsdaztp3_lw |Inheritance &amp; Polymorphism (Bana.14)|
|https://www.youtube.com/watch?v=1PPDoAKbaNA |Interfaces & Abstracts (Templates, Bana.15)|
|https://www.youtube.com/watch?v=h2tVne5nDUg |Class & Objects (Bana.16)|
|https://www.youtube.com/watch?v=AozJ0CR2W4A |What does "new" do (Telusko)|
|https://www.youtube.com/watch?v=VyPFa1Slh7A |New Operator (Ross)|
|https://www.youtube.com/watch?v=3c9SrLaMFGY |Static variable (Slidenerd.41)|
|https://www.youtube.com/watch?v=UhTF9MgyiiE |Static method (Diaz.09)|

### Optional
| Link | Comment |
|:---- |:------ |
|https://www.youtube.com/watch?v=rTSN-6bsa6k |Comparison of languages|
|https://www.youtube.com/watch?v=TeKTxG9DdQA |Inheritance, another perspective (EJ.14)|
|https://www.youtube.com/watch?v=H6Aaxle8DE4 |Interfaces, more examples to understand inheritance (Posch.01-4)|


## Assignment Review
*TBA.*

## Topics

### Fundamentals of OO
- Encapsulation
- Inheritance
- Polymorphism

### Classes &amp; Objects
- Conventionally named to start with a capital letter
- Consists of 
  - attributes (variables)
  - methods
- Core method is the constructor
  - what is happens when an *instance* (aka *extension*) of the class *intention* (aka *blueprint*) is called
  - can be overloaded
- Has other attributes, inherited from the Object class
  - HashCode()
  - getClass()

### This
- Provides the *blueprint* with a way to reference the *instance* inside of a Method definition.
- Looks like an Object reference

### Declaration types
- public
- protected
- private
- static

### Objects
- Is a *complex* variable (e.g. not a primitive)
- Is usually created with the *new* expression (NB. Strings)
- Is *passed* as a reference (not copied)

### Inheriting
How Java builds upon a progenitor class.  Creating a sub class from a parent.
- Exposes public and protected methods and attributes
- Means to add new methods and attributes (which can be further inherited)
- Overrides methods
- super() - means to refer the parent class (as opposed to &quot;this&quot;)

### Abstract
- Enforces the definition of base function and properties
- Can have some methods defined while demanding those that extend define the abstract methods

### Interface & Implements
- Workaround for inheriting from multiple classes
- Has no working code itself
- Convention expects the interface to start with &quot;I&quot;

### Main()
Let's re-examine `main()`
- Java only ever recognizes 1 `main()` 
  - usually marks the *lead* class (notice in the videos, for example, in each Bana lesson, he redefines main())
  - only has 1 way of being referenced (cannot be overloaded)
- Recognize it's called `void` and `static`

### Object datatype
- Concepts: 
  - utility - what are the benefits
  - what does it know (underlying datatype)
  - is a pointer
  - primitive vs complex datatypes
- Can be boxed and unboxed  

## Workshop/Practice 

### Challenge 
Ideas
- Create base class
- Do something where one needs to use this.
- Something needing to play with super()
- Override a method
- 2 types of constructors
- Implement an Abstract class
- static

## Assignment

# Links
- [Return to Module Overview](..)
- [Previous day](../../module-03/m03d4)
- [Next day](../m04d2)