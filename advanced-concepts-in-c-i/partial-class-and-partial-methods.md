# Partial Class and Partial Methods

In C#, you can split the implementation of a class or structure or a method or an interface in multiple.cs files using the partial keyword.&#x20;

The compiler will combine all the implementation from multiple.cs files or multiple CS files with the same name when the program is compiled.&#x20;

We use the partial keyword to build the partial class which can be compiled and combine as per the implementation and need individual term applications.&#x20;

<figure><img src="../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

This is the syntax of creating a partial class. We just add a partial keyword along with the class declaration.&#x20;

Partial classes comes into the picture when multiple developers can work simultaneously in the same class, in different files and they can be combined in the main iteration and location.&#x20;

You can split the UI of design code to read and understand the code where one developer can work at the server-side integration and another can work at the UI part.&#x20;

When you were working with automatically generated code, so some of the code is automatically generated in one of the partial class with the same component unless the user can customize and write.&#x20;

The code can be added to class without having to recreate the source file like visual studio. But yes, there is a drawback to when you modify one partial class, another gets automatically modified,&#x20;

You can also maintain your application in an efficient manner by comprising large classes into small units. To make it more intellectual, you also need to introduce the partial methods.&#x20;

<figure><img src="../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>



