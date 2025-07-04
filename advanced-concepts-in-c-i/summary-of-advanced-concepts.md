# Summary of Advanced Concepts

This Repository is to save the snippets of basics of programming in C#

## Partial Classes & Partial Methods

Partial classes and partial methods, all partial methods help us to split the code into different iteration

## Static Class

A static class is basically the same as a non-static class, but there is one difference: a static class cannot be instantiated. In other words, you cannot use the new operator to create a variable of the class type. [Microsoft](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/static-classes-and-static-class-members)

## Extension Methods

Extension methods are a form of syntactic sugar providing the illusion of adding new methods to the existing class outside its definition. In practice, an extension method is a static method that is callable as if it were an instance method; the receiver of the call is bound to the first parameter of the method, decorated with keyword this:

[Microdoft](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/extension-methods)

## Partial Class

A partial class is a class declaration whose code is divided into separate files. The different parts of a partial class must be marked with keyword partial.

[Microsoft](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/partial-classes-and-methods)

## Partial Methods

A partial class or struct may contain a partial method. One part of the class contains the signature of the method. An implementation can be defined in the same part or another part.
