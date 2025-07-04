# Classes and Objects

## Class

<mark style="color:purple;">A class is a blueprint or a template for creating objects</mark> and it defines the <mark style="background-color:purple;">data members</mark> and <mark style="background-color:purple;">member functions</mark> inside it, <mark style="color:purple;">which can be accessed with the help of an object.</mark>&#x20;

A class can also have fields, properties, and events. Depends upon what are the iterations and the expectations from the code.&#x20;

They collectively define the data and behavior of an object that can be accessed with the help of an instance that will be declared or defined within the class or outside the class definition.&#x20;

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

This is the syntax of declaring a class. First, we mention the access specifier, then the class keyword and the name of the class.&#x20;

Within the class, the member functions and member variables, which are the attributes and the behaviors needs to be defined for a specific entity.&#x20;

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<mark style="background-color:orange;">If we don't have any values assigned into it, they will be assigned with the default values because each and every class is inherited from the object class that defines the default values. Assign the default values to the data members if it is integer than zero, and if it is string, then null.</mark>&#x20;

## Objects

<mark style="color:purple;">Object is a dynamically created instance of the class that helps in accessing the members of a class from within the class or outside the class definition</mark>.&#x20;

The object definition starts with the <mark style="color:green;">class name</mark> followed by the <mark style="color:yellow;">object name</mark> and will be created with the help of a <mark style="color:orange;">new operator</mark> because it is a reference type.&#x20;

This is the syntax of creating object of a class. Here, <mark style="background-color:purple;">name of the object is nothing but a</mark> <mark style="color:orange;background-color:purple;">reference variable.</mark>

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

In this Program.cs, I will be instantiating my student class with this syntax. Post that student.accept detail or a display detail, whichever method you have.&#x20;

<mark style="background-color:purple;">But you can see that I'm not able to access this because all the members of my class are by default encapsulated. If I want to access this displayDetail from outside the class definition, I need to make it public.</mark>&#x20;

<mark style="color:purple;">Public is an access modifier.</mark> Here, I can access the displayDetail.&#x20;

If you have any other member function, which is acceptDetail, for example public void acceptDetails, that can accept the detail from the user.&#x20;

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

Let's say Console.Write, enter student Id. Here, I can read this and assign this to the student Id, studentId equals to Console.ReadLine.&#x20;

But <mark style="background-color:red;">everything that you take as an input in C# is in string format</mark> that will not store integer type, so you need to pass this into the integer type, whatever input you take from the user.
