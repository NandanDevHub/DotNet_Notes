# Summery of Abstarct Classes & Interfaces

## **Abstract Class**

The [abstract](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/abstract) keyword enables you to create classes and [class](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/class) members that are incomplete and must be implemented in a derived class.

Classes can be declared as abstract by putting the keyword abstract before the class definition

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members" %}

## **Interface**

Interfaces are data structures that contain member definitions and not actual implementation. They are useful when you want to define a contract between members in different types that have different implementations. You can declare definitions for methods, properties, and indexers. Interface members are implicitly public. An interface can either be implicitly or explicitly implemented.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/interface" %}

## **Interface vs. Abstract Class**

Interfaces and abstract classes are similar. The following describes some important differences:

* An abstract class may have member variables as well as non-abstract methods or properties. An interface cannot.
* A class or abstract class can only inherit from one class or abstract class.
* A class or abstract class may implement one or more interfaces.
* An interface can only extend other interfaces.
* An abstract class may have non-public methods and properties (also abstract ones). An interface can only have public members.
* An abstract class may have constants, static methods and static members. An interface cannot.
* An abstract class may have constructors. An interface cannot.

{% embed url="https://www.geeksforgeeks.org/difference-between-abstract-class-and-interface-in-c-sharp/" %}

\
