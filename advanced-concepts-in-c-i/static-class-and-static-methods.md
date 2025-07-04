# Static Class and Static Methods

Static class is basically the same as non-static class, but there is one difference, <mark style="background-color:purple;">a</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">**static class cannot be instantiated**</mark>**, means we cannot use&#x20;**<mark style="color:red;">**new**</mark>**&#x20;keyword to create an object of the class.**&#x20;

Even we cannot create any parameterized constructor because to pass the constructor value, we need to create an object.&#x20;

**Why do they use static in that scenario?** \
Because static means something which cannot be instantiated so it does not belongs to object as all the members of the static class even this static class itself will be accessible by the name of the parent iteration.\
<mark style="background-color:purple;">**For example, static methods and static variables can be accessed with the help of the class name rather than instance.**</mark>&#x20;

C-sharp static class cannot contain the instance constructors it contains these static constructors.&#x20;

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption><p>Apply static modifier before the class name or before the method name or the variable name makes them static and this is how the static class declaration works. </p></figcaption></figure>



<figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

Here is an example. We have a calculator class.&#x20;

Calculator class itself is static in-between we have a result storage initialized with zero.&#x20;

The number of times I will be changing its value or whenever I will access this result storage with the help of this calculator class that has calculator.\_resultstorage every class or every member will have the same value.&#x20;

That is how the statics sum and store methods are there so they will be actually calling with the help of a calculator.sum or calculator. Calculator.storage.&#x20;

## Advantages of Static Class

There are certain features and advantages of static class.&#x20;

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

Here I'm going to create a calculate class.

```csharp
using System;
namespace CSharp_Programming
{
	static class Calculate
	{
		//int count = 0;
		// Above This will give you error of instance member in static class

		public static int count = 0;

		//Calculate() { }
		// Above will give you error as Static classes cannot have instance constructors

		static Calculate()
		{
			count = 0;
		}

		public static int increment()
		{
			count++;
			return count;
		}

		public static int decrement()
		{
			count--;
			return count;
		}
	}
}


```

\
Below is how the members of the static class gets accessed. Even though if you would like to access console.write line, which is the object or a variable of static class that is calculate.count you can access it&#x20;

```csharp
// Static Classes
Console.WriteLine("----------------------Static Classes------------------------");

//Calculate calculate = new();
// Above will give the error as -  We cannot create an instance of static class


Console.WriteLine(Calculate.count); // Accessing Static Variable

Console.WriteLine(Calculate.increment()); // Accessing Static Methods
Console.WriteLine(Calculate.increment());
Console.WriteLine(Calculate.increment());

Console.WriteLine(Calculate.decrement());

```

<mark style="color:orange;">We generally use this in our scenario where one of the property of an entity needs to be shared across all the instances such as employees works in a particular organization and all the people share the same organization mean so in that case, we keep that variable as static.</mark>
