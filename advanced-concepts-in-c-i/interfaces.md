# Interfaces

<mark style="background-color:blue;">The interface in C# is a fully unimplemented class.</mark> Because it is used for declaring a set of operations or methods of an object in a particular class.&#x20;

We can define an interface as a pure abstract class that is a fully unimplemented class, which allows us to define only and only abstract methods.&#x20;

<figure><img src="../.gitbook/assets/image (104).png" alt=""><figcaption><p>We can use interface keyword to create an interface and this is how the interface is declared. </p></figcaption></figure>

You can see that to calculate area is not defined as an abstract method because what I said is interfaces are fully unimplemented class.&#x20;

By default, all the methods are abstract and public and interface itself says that I'm completely unimplemented class, behaves like an interface. We call interface is a purest form of contract that the concrete class always needs to implement.&#x20;

On the Right side of image as we can see&#x20;

* Rectangle is the name of the interface.&#x20;
* Interface starts with I, generally in most of the programming languages, but it is completely your choice.&#x20;
* <mark style="color:orange;">We cannot use access modifier inside an interface because by default the methods are public, which has a higher accessibility.</mark>&#x20;
* All members of an interface are public by default and also abstract and interface doesn't allow the fields.&#x20;

<mark style="background-color:red;">**Concrete Class - basically a class which is overrided**</mark>

<figure><img src="../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

* Interface specifies what a class must do and not how. Must do means the concrete classes needs to overwrite and then they should define the question that says, how?&#x20;
* Interface can't have private members because that needs to be used in the concrete classes. By default, all the members of interface are public and abstract.
* Interface cannot contain fields (body) because they represent a particular implementation of the data.&#x20;
* Earlier we have seen that a class can inherit only one class at a time, but a class can inherit one or more interfaces at a one given point of time, thus, multiple inheritance is possible with the help of interfaces, but not with classes where a child can have more than one parent.&#x20;

## Advantages of interfaces

<figure><img src="../.gitbook/assets/image (107).png" alt=""><figcaption><p>These are the higher advantages of interfaces</p></figcaption></figure>

* It is used to achieve loose coupling, which is a separation of concern.
* It is used to achieve total abstraction that a concrete class will access.&#x20;
* To achieve component-based programming&#x20;
* To achieve multiple inheritance and abstract in programming.&#x20;
* Interfaces add a plugin play-like architecture into the application, which can be easily injected into the other components that also helps in dependency injection.&#x20;

```csharp
using System;
namespace CSharp_Programming.Interfaces
{
	public interface IBankAccount
	{
		void deposit();

		void withdrawal();

		void savings();
	}
}


```

Just like we have bank account class, which has an abstract method BankAccount, we had an abstract methods deposit, withdrawal and savings, keeping it into my interface. But you don't need to define public and abstract, although there is no error in that.&#x20;

But <mark style="color:yellow;">**if you do not define public and abstract by default, all the methods of an interface are by public and abstract.**</mark>&#x20;

<mark style="background-color:blue;">**Multiple inheritance is possible with interfaces.**</mark> Let's say I have one more interface, IManagedBank. When I say I have IManagedBank, I have open account abstract method and close the account abstract method.&#x20;

```csharp
using System;
using CSharp_Programming.Interfaces;

namespace CSharp_Programming
{
    public class NewSavingsAccount : IBankAccount, IManageAccount // Multiple Inheritance
    {
        public void closeAccount()
        {
            Console.WriteLine("Account Closed");
        }

        public void deposit()
        {
            Console.WriteLine("Money Deposited");
        }

        public void openAccount()
        {
            Console.WriteLine("Account Opened");
        }

        public void savings()
        {
            Console.WriteLine("Money Saved");
        }

        public void withdrawal()
        {
            Console.WriteLine("Money Withdrawaled");
        }
    } 
}


```

I can say this saving account implements IBankAccount and IManageBank. That is completely possible. The moment we implement two interfaces in saving account,&#x20;

```csharp
NewSavingsAccount newSavingsAccount = new();

newSavingsAccount.deposit();
newSavingsAccount.closeAccount();
```

Here you go in program.cs. Creating an instance of saving account that is from interfaces.&#x20;

This is how the interfaces can be implemented in C#. Interface is a strict or a fully unimplemented class or contract that needs to be implemented in the concrete class.&#x20;

This is how the multiple inheritance can be achieved where a class can inherit one class or multiple interfaces at a given point of time.
