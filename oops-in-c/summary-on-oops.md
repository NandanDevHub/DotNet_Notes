# Summary on OOPS

## **Object-Oriented Programming Concepts**

C# has direct support for object-oriented programming.

### **Objects**

An object is created with the type as a template and is called an instance of that particular type.

In C#, objects are either references or values. No further syntactical distinction is made between those in the code.

### **Classes**

Classes are fundamentals of an object-oriented language such as C#. They serve as a template for objects. They contain members that store and manipulate data in a real-life like way.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/" %}

### **Access Modifiers**

Modifiers are keywords used to modify declarations of types and type members. Most notably there is a sub-group containing the access modifiers.

The access modifiers, or inheritance modifiers, set the accessibility of classes, methods, and other members. Something marked public can be reached from anywhere. private members can only be accessed from inside of the class they are declared in and will be hidden when inherited. Members with the protected modifier will be private, but accessible when inherited. internal classes and members will only be accessible from the inside of the declaring assembly.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/access-modifiers" %}

### **Constructor**

A constructor is a special method that is called automatically when an object is created. Its purpose is to initialize the members of the object. Constructors have the same name as the class and do not return anything. They may take parameters like any other method.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/constructors" %}

### **Inheritance**

Classes in C# may only inherit from one class. A class may derive from any class that is not marked as sealed.

_**class A**_

_**{**_

_**}**_

_**class B : A**_

_**{**_

_**}**_

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/inheritance" %}

### **Methods**

Like in C and C++ there are functions that group reusable code. The main difference is that functions, just like in Java, have to reside inside of a class. A function is therefore called a method. A method has a return value, a name and usually some parameters initialized when it is called with some arguments. It can either belong to an instance of a class or be a static member.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/methods" %}

### **Structure**

Although classes and structures are similar in both the way they are declared and how they are used, there are some significant differences. Classes are reference types and structs are value types. A structure is allocated on the stack when it is declared and the variable is bound to its address. It directly contains the value. Classes are different because the memory is allocated as objects on the heap. Variables are rather managed pointers on the stack which point to the objects. They are references.



{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/struct" %}

### Q\&A

> **What is a method in object-oriented programming?**
>
> A method is a function that is associated with an object or class and can be called to perform a specific task.

> **What is a structure in object-oriented programming?**
>
> Structures are a type of user-defined data type that allow you to combine different data types into a single unit, similar to a class. However, in a structure, its members are public by default, while in a class, they are typically private or protected by default.

> **Constructors allocate Memory?**\
> Yes! Constructors are used to create objects and allocate memory for them.

> **What is the difference between a method and a function in object-oriented programming?**
>
> There are differences between methods and functions in OOPS and one of those differences is that <mark style="color:red;">**methods are associated with objects**</mark> <mark style="color:red;"></mark><mark style="color:red;">while functions are not.</mark> However, the terms are sometimes used interchangeably, especially in languages that do not make a clear distinction between them.

> **What is an abstract class in object-oriented programming?**
>
> An abstract class is a class that cannot be instantiated, and it is often used as a base class for other class

> **What is method overloading in object-oriented programming?**
>
> Method overloading involves creating new methods with the same name but different parameters, but it does not involve creating new methods from existing ones, creating new classes, or creating new objects.

> **What is the difference between a static method and an instance method in object-oriented programming?**
>
> A static method cannot be called on an object, while an instance method can only be called on an object of the class. An instance method can access non-static fields and methods of the class, while a static method can only access static fields and methods.
