# Strings and String Methods

## Strings & String class

* In C#, a string is a sequence of characters that is stored in <mark style="color:yellow;">System.String class</mark>, as well as it represents a group of characters that needs to be stored into a single variable.&#x20;
* Considering I have hello is a string that containing a sequence of characters 'h' 'e' 'l' 'l' and 'o'. Internally, it stores into a characters array, but stored into one single variable, that's a string variable.&#x20;
* We can perform many operation on strings such as concatenation, comparison, getting substring, search from the existing string, removing the extra white spaces with trim, as well as string character replacements.&#x20;
* In C#, <mark style="color:purple;">string</mark> is a keyword which is an alias for <mark style="color:yellow;">System.String class</mark>.&#x20;
* <mark style="color:yellow;">System.String is a base class</mark>. That is why string and String, that is a string class are equivalent, we are free to use any naming convention.

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

* &#x20;Above are the syntaxes to declare or initialize this string. Here I have s1 that is creating string using string keyword, and another is declaring a string with the help of a String class itself.

## Types of Strings

* We have two types of strings in C#, one is a <mark style="color:orange;">immutable string</mark> and another is a <mark style="color:purple;">mutable string</mark>.&#x20;
* String declared from <mark style="color:yellow;">System.String class</mark> are <mark style="color:orange;">immutable</mark>, which means we are creating a new memory every time instead of working on existing memory. Whenever we are modifying a value in the existing string, also, we're creating a new object which refers to that modified string, and the old one becomes unreferenced.&#x20;

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* But in the case of mutable string, there is a <mark style="color:green;">StringBuilder class</mark>, which is <mark style="color:purple;">mutable</mark> type. That means if we are using the same memory location and keeping the stuff to the one instance, it will not create any further instances, hence it will not decrease the performance of the application.&#x20;
* We prefer to use <mark style="color:green;">StringBuilder clas</mark>s, whenever we are really sure that we would like to append and modify the stuff of the string value.&#x20;
* In conclusion, <mark style="color:purple;">mutable strings</mark> can be append or it's modifiable, while <mark style="color:orange;">immutable strings</mark> can't be modified.&#x20;

## String Methods

* In System.String. We have these functions associated with it, Clone, CompareTo, Contains, EndsWith, Equals, ToUpper, ToLower, Insert, and IndexOf.&#x20;

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

As it is easily suggested above,&#x20;

1. Clone is to make a copy of the string.
2. CompareTo, is to compare two strings and return integer value if the strings are equal or not.
3. Contains, to check whether a specified character exist or not in the string value.
4. EndsWith, to check whether our strings ends with a specific character that we can check with EndsWith.
5. Equals is to compare two strings and return the Boolean value as output, true or false.&#x20;
6. ToUpper and ToLower converts the string to uppercase or lowercase, respectively.&#x20;
7. Insert, inserts a string or a character in the string at a specified position as a substring.
8. IndexOf is to return the index position of the first occurrence of a specified characters from the existing string as well.
