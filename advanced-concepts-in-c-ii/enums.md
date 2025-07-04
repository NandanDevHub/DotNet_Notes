# Enums

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

An enum is a user-defined datatype that has a fixed set of related values. It is used to assign constant names to a group of numeric integer values and it also makes constant values more readable,

For example we have weekdays where weekdays start from Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, and ends up on Sunday. We have different genders like male, female, or unknown. We have four different directions, South, East, West, and North. Depends what are their specific range of the input values on the basis of which you would like to give the accessibility.

&#x20;Whatever you access with the help of the dot operator, even in programming is also known as enumaration. Above it's depicting only three months that is May, June and July.&#x20;

An **enum** is defined using enum keyword, as you can see here, directly inside the namespace, where the class is described. All the constant names can be declared inside the curly brackets as I can show you here.

```csharp
using System;
namespace CSharp_Programming
{
	enum WeekDays:byte
	{
		Monday,
		Tuesday = 33, // Re-assign their values
		Wednesday,
		Thrusday,
		Friday,
		Saturday,
		Sunday
	}

	public class Enums
	{
        public void displayWeekDays()
		{
			Console.WriteLine(WeekDays.Friday);
			Console.WriteLine(WeekDays.Wednesday);

			//To get the integral value of what they represent
			int day = (int)WeekDays.Sunday; // Type of Interger Type
			Console.WriteLine(WeekDays.Sunday + ":" + day);

			day = (int)WeekDays.Tuesday;
			Console.WriteLine(WeekDays.Tuesday + ":" + day);
		}
	}
}
```

This is how enumeration works in a real-time implementation to give you a support where the list can be accessed with the help of the dot operator
