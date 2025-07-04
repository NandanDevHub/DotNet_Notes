# Extension Methods

Extension methods, as the name suggests, are additional methods that needs to be added with each and every iteration and the variable that we can access with the help of the dot operator.

<mark style="background-color:yellow;">Basically Extension Methods wo methods hai like tum custom define kr skte ho tumhe kuch krna hai toh and wo tum directly us kr skte ho, jaise kuch inbuilt function hote hai waise, for exmaple - IsNullOrEmpty wala jo hai wo Extension Method hi toh hai.</mark>

&#x20;Extension method allows you to inject additional methods without modifying or recompiling the original class structure or interface.&#x20;

They are the special type of the static method that can be called as an instance methods.&#x20;

Extension methods can be added to your own custom class,.NET Framework classes, or third-party classes or interfaces.&#x20;

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

This is one of the example. Here, i is one of the variable and is greater than the extension method that can be accessed with the help of the dot operator.&#x20;

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

Considering I have a variable, integer number that is 314, I would like to store the boolean result based upon this extension method where I say that if my number is greater than, that is, is greater than 2000, then it will return true. Otherwise it will return false.&#x20;

```csharp
using System;
namespace CSharp_Programming
{
	static class CheckExtension
	{
		public static bool IsGreaterThan(this int i, int value)
		{
			return i > value;
		}
	}
}
```

You can see that is greater than method is not a method of int datatype. It is an extension method returned by the programmer.&#x20;

What I will be doing is I will be creating is greater than method inside the  Check extension, so that it will be accessible with integer type. I'll make this class as static.&#x20;

Inside this, I will be creating a static bool return type is greater than, which will take this integer, the value of number which will be assigning into the number and the value by which you are comparing it.&#x20;

Post that. I would be doing the comparison return i greater than value. If i is greater than value or a number is greater than value, it means that it will return true, otherwise it will return false.&#x20;

```csharp
	public class ExtnMethods
	{
		 public int number = 314;
		bool result;

		public ExtnMethods()
		{
            result = number.IsGreaterThan(2000);
        }
	}
```

You can see that this extension method is applicable now.&#x20;



