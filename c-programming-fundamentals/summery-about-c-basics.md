# Summery about C# Basics

## **Introduction to C#**

* C# is a general-purpose <mark style="color:purple;">high-level programming language</mark> supporting multiple paradigms.
* The language is intended to be a simple, modern, general-purpose, <mark style="color:purple;">object-oriented programming language</mark>
* The language is intended for use in developing software components suitable for deployment in distributed environments.

{% embed url="https://www.guru99.com/c-sharp-tutorial.html" %}

## **History of C# Version**

* The C# programming language was designed by Anders Hejlsberg from Microsoft in 2000 and was later approved as an international standard by Ecma in 2002.
* Microsoft introduced C# along with .NET Framework and Visual Studio and that time both were closed source.
* A decade later, Microsoft released Visual Studio Code, <mark style="color:orange;">Roslyn (compiler),</mark> and the unified .NET platform (software framework), all of which support C# and are free, open-source, and cross-platform.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-version-history" %}

## **C# Code Execution**

The core syntax of the <mark style="color:yellow;">C# language is similar to that of other C-style languages such as C, C++ and Java,</mark> particularly:

* Semicolons are used to denote the end of a statement.
* [Curly brackets](https://en.wikipedia.org/wiki/Curly_brackets) are used to group statements. Statements are commonly grouped into methods (functions), methods into classes, and classes into [namespaces](https://en.wikipedia.org/wiki/Namespaces).
* Variables are assigned using an [equals sign](https://en.wikipedia.org/wiki/Equals_sign), but compared using [two consecutive equals signs](https://en.wikipedia.org/wiki/%3D%3D).
* [Square brackets](https://en.wikipedia.org/wiki/Square_brackets) are used with [arrays](https://en.wikipedia.org/wiki/Array_data_structure), both to declare them and to get a value at a given index in one of them.

The following is a very simple C# program, a version of the classic "Hello world" example using the top-level statements feature introduced in C# 9

```csharp
using System;
Console.WriteLine("Hello, world!");
```

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/tutorials/hello-world" %}

## **Installing and Configuring Visual Studio**

* Visual Studio Code, also commonly referred to as VS Code is a source-code editor made by Microsoft with the Electron Framework, for Windows, Linux and macOS.
* In the below video, we will install and configure visual studio for code implementation.

{% embed url="https://learn.microsoft.com/en-us/visualstudio/install/install-visual-studio?view=vs-2022" %}

## **Variable**

* Variables are identifiers associated with values.They are declared by writing the variable's type and name, and are optionally initialized in the same statement.
* Refer to below link to know more about variables in C#.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/variables" %}

## **Data Type**

C# has a unified type system. <mark style="color:purple;">This unified type system is called Common Type System (CTS</mark>).

A unified type system implies that all types, including primitives such as integers, are subclasses of the `System.Object` class. For example, every type inherits a `ToString()` method.

CTS separates data types into two categories:

* Reference types
* Value types

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/types" %}
