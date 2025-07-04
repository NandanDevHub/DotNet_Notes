# C# Arrays & Strings

Two important data structures in the C# programming language.



1. <mark style="color:purple;">Single Dimensional Arrays:</mark> \
   This is the most common type of array in C#. It is a collection of elements of the same data type arranged in a single row. You can access individual elements using their index position. For example, `int[] numbers = new int[5];`creates an array of integers with a length of 5.
2. <mark style="color:purple;">Multidimensional Arrays:</mark> \
   These arrays have more than one dimension, allowing you to store data in a tabular form. The most common type is a two-dimensional array, which is like a matrix with rows and columns. You can access elements using two indices. For example, `int[,] matrix = new int[3, 3];` creates a 3x3 matrix.
3. <mark style="color:purple;">Jagged Arrays:</mark> \
   A jagged array is an array of arrays. Each element of the main array can be an array of different lengths. This allows you to create arrays with varying sizes. You can access elements using two indices, just like a multidimensional array. For example, `int[][] jaggedArray = new int[3][];` creates a jagged array with 3 rows, where each row can have a different number of columns.
