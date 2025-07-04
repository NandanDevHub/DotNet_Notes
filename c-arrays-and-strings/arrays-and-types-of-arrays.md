# Arrays and Types of Arrays

## Array

<mark style="color:orange;">Array</mark> is the most important concept to be discussed in programming language.&#x20;

Considering a <mark style="color:purple;">variable</mark> is used to store a <mark style="color:purple;">literal value</mark> where an <mark style="color:orange;">array</mark> is used to store <mark style="color:orange;">multiple literal values.</mark>&#x20;

That is called a collection of elements of same data type that are stored in contiguous memory location.&#x20;

Each element in an array is identified by its index or position within the array, starting from zero. Considering if the size of the array is n, then index element starts from zero and ends at n minus 1. See below:

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

Arrays are declared using square bracket after the data type name, followed by the array name. This is the syntax of declaring an array that holds five integers.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

## Advantages of Arrays

Advantages -&#x20;

* This helps in code optimization by writing less code rather than declaring multiple variables.&#x20;
* We declare one variable with a specific size. We can randomly access the array elements.&#x20;
* Easy to traverse the data based upon the index or the iterations.&#x20;
* Easy to manipulate or modify the existing data as well,&#x20;
* Arrays is one of the class in C# that helps in sorting the data and arranging the data in different orders.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

## Types of arrays in C\#

Types of Array

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

## One Dimensional Array

The single-dimensional array is also known as one-dimensional array.

It is the simplest form of declaring an array that contains only one row for storing the homogeneous data.&#x20;

It has single set of square brackets.

To declare single-dimensional array in C#, There are different syntaxes, Below we have declare age array.&#x20;

Here I'm going to allocate the size to the array and we can also do this into one line by not writing this assignment and directly writing here age equals to new integer 5. Even though we can initialize the array elements in it in the single line depends upon the requirement you would like to declare the array or you would like to initialize the array.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

### Multi-dimensional array

Multi-dimensional array is the array that contains more than one row to store the data in it.&#x20;

It is also known as a rectangular array because it has the same length of each row.&#x20;

Some people consider this as a <mark style="color:orange;">matrix</mark> to be declare where the row and columns needs to be defined.&#x20;

It can be two-dimensional array or three-dimensional array depends upon the requirement.&#x20;

But in the case of multi-dimensional, <mark style="color:orange;">minimum of two dimensions are required.</mark>&#x20;

In C#, we can separate multi dimensions with the help of <mark style="color:orange;">comma.</mark>&#x20;

This is the example how you can define your multi-dimensional array.&#x20;

```csharp
int [,] s = new int [3,3]
```

Here this array name is s, and this is going to store three rows and three columns. The <mark style="color:orange;">first dimension is basically four rows,</mark> and the <mark style="color:orange;">second dimension is basically four columns.</mark>&#x20;

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

This is how the index elements are iterated. Here you can see that in the first row, index is zero, but column is frequently changing. In this second row, index is one and the column is frequently changing, starting from zero till n minus 1, that is 2. The same where it happens in the third row that is index 2, and column is frequently changing, that is starting from zero and get ends by n minus 2.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

### Jagged Array

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

Jagged array is an area of arrays where <mark style="color:orange;">each sub-array can have a different length.</mark>&#x20;

Basically, jagged arrays are useful when you need to store a collection of <mark style="color:purple;">arrays of different sizes</mark> and it is initialized with two square brackets.&#x20;

The <mark style="color:orange;">first bracket specifies the size of an array,</mark> and the <mark style="color:orange;">second bracket specifies the dimensions of the array which is going to be stored.</mark>&#x20;

You can see that I will be creating three arrays. The second bracket depicts the number of elements I'm going to store in each array. Each array has a different dimension length that is to be considered in the jagged array.&#x20;

The jagged arrays basically depict the arrays of arrays where the <mark style="color:purple;">second dimension can be single-dimensional or multi-dimensional array.</mark> But the first dimension, first square bracket, will always tells you how many parent arrays you can consider into the jagged array.
