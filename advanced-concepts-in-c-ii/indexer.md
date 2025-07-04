# Indexer

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

* An indexer can be defined with the same way as property with **this** keyword along with the square bracket.&#x20;
* A one-dimensional indexer has this particular syntax, given above, First, we write the element type, **this** keyword, and then the index name. Along with that, we put get and set that returns the value from a specified index of an internal collection or then sets the value at the specified index in an internal collection.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

```csharp
using System;
namespace CSharp_Programming
{
	public class StringIndexerType
	{
		private string[] strArray = new string[10];

		public string this[int index]
		{
			get
			{
				if (index < 0 || index >= strArray.Length)
					throw new ArgumentOutOfRangeException("Index is out of range");
				return strArray[index];
			}

			set
			{
				if (index < 0 || index >= strArray.Length)
					throw new IndexOutOfRangeException("Index is out of range");
				strArray[index] = value;
			}
		}
	}
}


```

