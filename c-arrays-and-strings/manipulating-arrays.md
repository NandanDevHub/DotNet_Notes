# Manipulating Arrays

One Dimensional Array Manipulation

```csharp
// You can assign values at the time of declaration as below 
int[] student = new int[5] {41,76,75,13,47}; // This is called initialization

			// This is one way to assign values
			//student[0] = 41;
			//student[1] = 76;
			//student[2] = 75;
			//student[3] = 13;
			//student[4] = 47;
			

			foreach(int marks in student)
			{
				Console.WriteLine("THe Marks of Students are:" + marks);
			}
```

## Two Dimensional Array Manipulation

```csharp
int[,] rando = new int[2, 3] { { 23, 54, 54 }, { 87, 12, 68 } };

			//foreach ( int marks in rando)
			//{
   //             Console.WriteLine("THe New Marks of Students are:" + marks);
   //         }

			for(int i = 0; i<=1;i++)
			{
				for(int j=0; j<3; j++)
				{
					Console.Write(rando[i, j] + "\t");
				}
				Console.WriteLine();
			}
```

## Jagged Array Manipulation

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>
