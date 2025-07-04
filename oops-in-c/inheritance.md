# Inheritance

### Inheritance

It is possible to inherit the fields and methods from one class to another, where the one class is the superclass and another is the subclass.&#x20;

It allows us to define a new class based on an existing class, where it helps in re-usability of the code.

The new class inherits the properties and methods of the existing class, that is the base class, and can also add the new properties and methods of it's own.&#x20;

It promotes code reuse and simplifies the code maintenance, also it helps in reducing the time and efforts of a programmer.&#x20;

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

For example, there is a vehicle.&#x20;

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

One vehicle is the parent class. Every vehicle has speed, every vehicle has other properties like color and all. But bike, car, buses, and trucks has different things, functionalities.&#x20;

Along with that, bike, cars and buses and trucks do have the different number of wheels. Along with that, the bike has certain categorized into scooter and the bicycles. Where the scooter has gears or other functionalities where the cycle is not having those features.&#x20;

<mark style="color:purple;">Common functionalities can be kept in a vehicle class</mark> and other bikes, functionalities can be kept in the bike class. <mark style="color:purple;">So whatever common functionality we have in this vehicle class can be reused in the such bikes, cars, bus, and trucks class.</mark>&#x20;

<mark style="background-color:orange;">This is how the inheritance can only be used with related classes where they should have some common behaviors and perfect substitutable.</mark>&#x20;

## Types of Inheritance

We have different types of inheritance.&#x20;

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

Whenever we talk about inheritance, there are two classes comes into the picture, <mark style="color:purple;">**base class**</mark> and <mark style="color:orange;">**derived class.**</mark> <mark style="color:purple;">Base class</mark> can also be known as a <mark style="color:purple;">**superclass**</mark>. In that case, the <mark style="color:orange;">derived class</mark> will known as a <mark style="color:orange;">**subclass**</mark>.&#x20;

### Single inheritance.&#x20;

When we have only one <mark style="color:purple;">parent class</mark> and one <mark style="color:orange;">child class</mark>, that is inherited the last A into the class B, so class B can access the behaviors of class A, that is known as a single inheritance.&#x20;

### Multilevel Inheritance

In the case of multiple inheritance, class A inherits to B and B inherits to C. Indirectly, class A inherits to C as well. That is a multi-level inheritance.&#x20;

### Hierarchical Inheritance

When Class A inherits to class B and class A inherits to class C. That is a hierarchical or tree inheritance. <mark style="color:yellow;">There is no association between class B and class C with each of them.</mark>&#x20;

### Hybrid Inheritance

Hybrid inheritance can have any kind of pattern.&#x20;

### Multiple Inheritance

Multiple inheritance says that one child class or one derived class will have multiple parents.&#x20;

<mark style="color:red;">**That can not be achieved in C# at all.**</mark> It can be achieved with the help of interfaces, that is the add-on functionality to the object-oriented programming<mark style="color:orange;">. But it is not possible with the help of classes, because</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**one class can inherit only one class in the C# at a given point of time.**</mark>&#x20;

```csharp
public class Marks :Student
// Here Marks is child class and Student is parent class
{
    float objectiveMarks;
    float subjectiveMarks;
    .
    .
}    

```

When I will be instantiating my Marks class, I will be instantiating my marks class. The moment I will be instantiating my child class, the memory gets allocated to the data member of the parent class as well as child class.&#x20;

If you would like to call your parent class accept detail and display detail also, so what will happen, from this accept detail you are calling your marks accept detail. Either give a different name to the accept detail and display detail of each class. But if you are giving the same name, this is going to call the accept detail of the marks.&#x20;

```csharp
	//Single Inheritance
	
	public class Marks :Student
	{
		float objectiveMarks;
		float subjectiveMarks;

        public void displayDetails()
        {
            base.displayDetails(); // This will first call Parent class
            Console.WriteLine("Objective Marks are " + objectiveMarks);
            Console.WriteLine("Subjective Marks are " + subjectiveMarks);
        }

        public void acceptDetsils()
        {
            base.acceptDetsils(); // This will first call Parent class
            Console.WriteLine("Enter The Objective Marks:");

            objectiveMarks = float.Parse(Console.ReadLine());

            Console.WriteLine("Enter the Subjective Marks");
            subjectiveMarks = float.Parse(Console.ReadLine());

            Console.WriteLine();
        }
    }

```

First it will call the parent class, accept detail will execute that and that then will come and execute these statements. Same thing will happen with base.displayDetails.&#x20;

The Sequence would be like First, it will call the accept detail of the parent class. Then it will execute the accept detail of the child class of its own. In the same fashion it will execute the display detail of the child class as well. This is how single level inheritance works.
