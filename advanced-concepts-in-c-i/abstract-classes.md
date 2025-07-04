# Abstract Classes



## Abstract Class

An abstract class is a class that cannot be instantiated or we <mark style="background-color:blue;">cannot create an object of a class if</mark> the class is abstract. Instead, it serve as a base class for the other concrete classes to inherit from. They are used to define a common set of properties that derived classes should have.&#x20;

In short, we can use abstract classes as a contract that needs to be implemented by these subclasses or concrete classes. Here, I'm using a term concrete classes.&#x20;

**Concrete class** is a class, which is not an abstract class or a contractual class to be used in programming. <mark style="background-color:blue;">Abstract keyword is used to create an abstract class</mark>.&#x20;

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption><p>This is how an abstract class is created. </p></figcaption></figure>

The moment we keep this class as an abstract, we cannot create an object of this class or instantiate this class. It will throw an error to us.&#x20;

There is no other purpose of creating any classes in abstract. Whenever a class or a particular class contains the abstract methods, that class needs to be abstract.&#x20;

An abstract class can have both abstract methods and non-abstract method, which has a body.&#x20;

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

Above class which has an abstract method display1 without the definition, the non-abstract method that is display2.&#x20;

<mark style="background-color:blue;">The non-abstract method can be accessed with the instance of the</mark> <mark style="background-color:blue;"></mark><mark style="background-color:blue;">**child class**</mark>**.** A

## Abstract Method

<mark style="background-color:purple;">A method that does not have a body is known as an abstract method.</mark>&#x20;

* If we use abstract with any of the method, we should not define the body. That method automatically becomes the abstract.&#x20;
* One important thing, if a particular class contains any abstract method, that class has to be abstract. An abstract method must be declared in an abstract class only that needs to be implemented in the derived class. It is compulsion.&#x20;

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption><p>This is how an abstract class will have an abstract method demonstrated.</p></figcaption></figure>



```csharp
using System;
namespace CSharp_Programming
{

	//Abstarct Classes & methods
	public abstract class BankAccount
	{
		public abstract void deposit(); // Abstract Methods have no body

		public abstract void withdrawal(); // Abstract Methods have no body

        public abstract void savings(); // Abstract Methods have no body
    }

    public class SavingsAccont : BankAccount // Inheriting
    {
        public override void deposit() // Now we can access the abstract class methods
        {
            Console.WriteLine("Money in Deposit");
        }

        public override void savings()
        {
            Console.WriteLine("Money in Savings");
        }

        public override void withdrawal()
        {
            Console.WriteLine("Money Widhwrawaled");
        }
    }
}


```

Here, I'm creating a class BackAccount. This BackAccount class, I'm making it as an abstract class.&#x20;

* When i create abstract methods but not abstract class I'm still getting error because a class that consist the abstract method, that class also needs to be abstract.&#x20;
* If a class is abstract. There is no need of method body. If any class is having any abstract method, that class itself needs to be abstract. This is a contractual class.&#x20;
* Now Creating , I'm creating a saving account.  This saving account inherits the abstract class BackAccount. It is forced that the saving account needs to implement the abstract methods of the BackAccount. It means the overridden implementation needs to be there.&#x20;
* Here, I'm simply defining a body with a message, Console.WriteLine balance in saving account, etc
* &#x20;If abstract class can also contain non-abstract method, public void getMessage. This message just prints Console.WriteLine welcome to ABC Bank. This is the abstract class and we have non-abstract method in it. We cannot create the BackAccount object this way because it is an abstract class. An abstract class cannot be instantiated. What I can do is I can call this getMessage method with the help of a saving account method because it is the child class or a derived class of the BackAccount.
