# Summery on Jump Statements

## **Operators**

C# provides a number of operators. Many of them are supported by the built-in types and allow you to perform basic operations with values of those types. Those operators include the following groups:

* Arithmetic operators that perform arithmetic operations with numeric operands
* Comparison operators that compare numeric operands
* Boolean logical operators that perform logical operations with bool operands
* Bitwise and shift operators that perform bitwise or shift operations with operands of the integral types
* Equality operators that check if their operands are equal or not.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/" %}

## **Operators precedence**

Operator precedence determines the grouping of terms in an expression.&#x20;

This affects evaluation of an expression. Certain operators have higher precedence than others;&#x20;

For example, the multiplication operator has higher precedence than the addition operator.

For example x = 7 + 3 \* 2; here, x is assigned 13, not 20 because operator \* has higher precedence than +, so the first evaluation takes place for 3\*2 and then 7 is added into it.

{% embed url="https://www.tutorialspoint.com/csharp/csharp_operators_precedence.htm" %}

## **Conditional Statements: if, if..else if, switch**

The if, if-else and switch statements select statements to execute from many possible paths based on the value of an expression.&#x20;

The <mark style="color:purple;">if s</mark><mark style="color:purple;background-color:purple;">tatement</mark> executes a statement only if a provided Boolean expression evaluates to true.

The <mark style="background-color:purple;">if-else</mark> statement allows you to choose which of the two code paths to follow based on a Boolean expression.&#x20;

The <mark style="background-color:purple;">switch statement</mark> selects a statement list to execute based on a pattern match with an expression.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/selection-statements" %}

## **Loops: do..while, while, for, foreach**

The iteration statements repeatedly execute a statement or a block of statements.&#x20;

The <mark style="color:purple;">for statement</mark> executes its body while a specified Boolean expression evaluates to true.&#x20;

The <mark style="color:purple;">foreach</mark> statement enumerates the elements of a collection and executes its body for each element of the collection.&#x20;

The <mark style="color:purple;">do</mark> statement conditionally executes its body one or more times. The <mark style="color:purple;">while</mark> statement conditionally executes its body zero or more times.

At any point within the body of an iteration statement, you can break out of the loop using the break statement. You can step to the next iteration in the loop using the continue statement.

{% embed url="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/iteration-statements" %}

## **Jump Statements**

In C#, Jump statements are used to transfer control from one point to another point in the program due to some specified code while executing the program.

{% embed url="https://www.geeksforgeeks.org/c-sharp-jump-statements-break-continue-goto-return-and-throw/" %}
