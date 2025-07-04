# Polymorphism

Polymorphism in C-sharp, one of the very important component in object-oriented programming. Polymorphism is driven from a Greek word that means multiple forms or shapes where poly means many, and morpho means forms.&#x20;

You can use polymorphism if you want to have multiple forms of one or more methods of a class with the same name.&#x20;

<figure><img src="../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure>

Considering by using inheritance, a class can be used as many times. Say, we have a person which may be a professor, maybe a student, or maybe a clerk. Person would be the parent class and in the child classes or child entities like professors, student, and clerk, their attributes can be redefined or their behaviors can be redefined with the same name.&#x20;

<figure><img src="../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

### Types of Polymorphism

In C-sharp polymorphism can be achieved in two ways.&#x20;

1. **Compile-time polymorphism** that is also known as static polymorphism&#x20;
2. **Runtime polymorphism** that is also known as dynamic polymorphism.&#x20;

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

When we derive a class from base class, it inherits all the methods, properties, fields, and events of the base class. To change the behavior or data of base class, we have two ways. Either we can hide the base method by using new keyword or override the base method by using override keyword.&#x20;

### Scenario

When one task is performed by different ways, then it is known as polymorphism.&#x20;

<figure><img src="../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>

There is a person, student, and millionaire also comes under a person category, but when it comes to the playbill, student pays the bill for his or her academics but a millionaire pays the bill for his or her credit amounts or maybe distribution of the salary.&#x20;

Everyone is paying their expenses or bills, but they have a different functionalities to be iterated and this iteration comes as an polymorphism, <mark style="background-color:blue;">one entity, one method, but different overridden functionalities</mark>.&#x20;



### Compile Time Polymorphism

In compile-time polymorphism the compiler <mark style="background-color:blue;">identifies which method is being called at the compile time.</mark>&#x20;

<figure><img src="../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

In C-sharp, compile-time polymorphism can be achieved in two ways -&#x20;

1. Method Overloading
2. Constructor Overloading.

#### Constructor Overloading

Constructor overloading, is where when a class can have more than one constructors just like we had default constructor and the parametrized constructor.&#x20;

#### Method Overloading

Method overloading is a mechanism to have more than one method with the same name but with different signature where signature is basically a parameter.&#x20;

If in a class we have more than one method with the same name, they must have&#x20;

* a different number of parameter&#x20;
* having same number and type of parameter but in different orders
* having same number of parameters but of different types.&#x20;

<mark style="background-color:orange;">Method overloading is also known as early binding or static binding</mark> because first the compilation happens and then the execution happens. That is what we also call compile-time polymorphism, early binding or static binding.&#x20;

In C-sharp, we can overload methods, constructors, and indexed properties. As per the requirement, you can really optimize in the pattern.&#x20;

You would like to overload the methods in the class, constructors in the same class, or the indexed properties. It is because these members have parameters and on the basis of different signature or different parameters, the methods, index properties, and constructors can be overloaded.&#x20;

<figure><img src="../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

This is how in one class we have method one with one parameter, another but two parameter of different types, and another with three parameters of different type or maybe same type.Here the number of parameters are different in each iteration.&#x20;

<figure><img src="../.gitbook/assets/image (101).png" alt=""><figcaption><p>This is the demonstration of method overloading. </p></figcaption></figure>

In the ConsolePrinter class, we have three print methods. One which has a string variable, string parameter, another we have two string parameter and another we have three string parameters. Here the parameters are different as number of parameters and each method with the same method name. That is how method overloading can be achieved.&#x20;

***

***

### Method Overriding

* Method overriding can be done  only in derived classes.&#x20;
* It means it cannot be implemented without inheritance.&#x20;
* It is used to achieve the runtime polymorphism where two or more classes comes into the picture.&#x20;
* It enables you to provide implementation of a method which is already provided by its base class and the child classes overrides or redefine their behaviors.&#x20;

<figure><img src="../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

Example - The one which I have demonstrated in the person example, where the student and millionaire were paying their bills, but student was paying their academic bill so their calculation is quite different, but millionaire is paying their credit card bills or maybe other finances or the salaries, so their calculation is quite different.&#x20;

You need to use <mark style="color:orange;">virtual</mark> keyword with the <mark style="color:orange;">base</mark> class method and <mark style="color:yellow;">override</mark> keyword with the <mark style="color:yellow;">derived</mark> classes depending on you what would you like to provide the new definition or remove the previous one

You can also use <mark style="color:red;">abstract</mark> If you don't want to remove the previous implementation, you can keep the method as virtual.&#x20;

#### Scenario -&#x20;

<figure><img src="../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

This is the example of animal class has a method called MakeSound. I have the Animal class MakeSound method and that I kept it <mark style="color:orange;">virtual</mark>. Once the Dog class <mark style="color:yellow;">overrides</mark> this MakeSound method and provides some new different implementation.&#x20;

When you will call your MakeSound method is with the Dog class object, it will bring the dog barks but when you will call the Animal MakeSound method with the animal object, it will print the message the animal makes a sound.

**If you don't want to provide the basic overridden implementation, which is the make sound of the animal rather than creating this method virtual, you can make it as in contract with the help of abstract method.**
