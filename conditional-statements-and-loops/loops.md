# Loops

## Loops

* In programming, it is often desired to execute a certain block of statements for a specific number of times.&#x20;
* A possible solution will be to type those statements for the required number of times.&#x20;
* The number of repetitions may not be known in advance during compile time, or maybe large enough, let's say 1,000, 10,000 or one lakh.&#x20;
* So loops are basically used to repeat a block of statements for certain times.&#x20;
* Variable can decide the number of times a loop has to be executed.&#x20;
*

<figure><img src="../.gitbook/assets/image (91).png" alt=""><figcaption><p>Flowchart of Loop</p></figcaption></figure>

This is how a flowchart works for the loop statements. When you enter into your program, the loop condition is to be checked if the loop condition is true, after printing the loop block or executing the loop block, it will again check the condition. Until the condition is true, the loop block will be executed and every time the condition will be checked. If the condition becomes false, it will exit out of the loop.

<figure><img src="../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

## Types of Loop

Every loop is implemented in their own iteration in a different way.

<figure><img src="../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:yellow;">**For loop and while loop are to be used when the number of iterations are fixed or certain.**</mark>&#x20;
* <mark style="color:yellow;">**When it is not certain you can use a do while loop**</mark>
* <mark style="color:yellow;">**Foreach is basically to iterate the collection or a collection of values that needs to be printed or iterated.**</mark>

### For Loop

&#x20;Array of String Types ;

```csharp
string[] names = new string[5] { "Shikhar Dhawan", "Rohit Sharma", "Virat Kohli", "Suresh Raina", "MS Dhoni" };
```

* I wanted to use a for loop where I say that there would be an iterative variable.&#x20;
* <mark style="color:red;">**You can name this variable anything, but we generally keep this variable name as i, because i stands for iteration.**</mark>&#x20;
* Then I'm saying that until i is less than names.Length. If you don't want to use this property and you know the fixed number of iteration, you can use five.

```csharp
string[] names = new string[5] { "Shikhar Dhawan", "Rohit Sharma", "Virat Kohli", "Suresh Raina", "MS Dhoni" };

// Now for iteration use can either use fixed number as 5 or can say as below :-
for (int i = 0; i<names.Length ; i++)
 {
  Console.WriteLine(names[i]); // Printing names at ith position.
 }
 
 // Similarly 
 
 // FOR LOOP - Reverse Order

for (int i = 4; i >= 0; i--)
  Console.WriteLine(names[i]);
```

### While Loop

* While loop also decided to be used when the number of iterations are known or fixed.
* The amazing part is the console statement gets printed and afterwards i needs to be incremented and decremented.&#x20;
* You can see that here the same initialization condition and increment and decrement is there but the syntax is different.

<pre class="language-csharp"><code class="lang-csharp">// While Loop

i = 0;
<strong>while (i &#x3C; names.Length)
</strong> {
   Console.WriteLine(names[i]);
i++;
}
			}
</code></pre>

### Do While Loop

Do\_while loop is a loop where we do not check for any condition at the first time. and from the second time onward, the loop condition is to be checked.

<mark style="background-color:orange;">That means the Loop will any 1 one time in anyhow and then the next time it will check the condition.</mark>

<mark style="background-color:orange;">Here in Do section - We will place the piece of code that we want to do. and in</mark> \ <mark style="background-color:orange;">WHile Section - We will add the condition on the basis if which it will execute do.</mark>

### For Each Loop

For each loop is specific to iterate the collection just like array I list and something more

```csharp
foreach(string name in names)
 Console.WriteLine(name);
```

#### Difference between for and for each

* For loop you could print this collection or the values in reverse order, that you cannot do with the help of foreach.&#x20;
* Foreach always gets printed in the incremental order by taking the value from the collection, assigning it to the variable and printing or whatever operation you wanted to do inside the loop.
* Wherever I would like to use collections, we'll give a priority to foreach loop

