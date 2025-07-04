# Conditional Statements

## Conditional Statements

* C Sharp provides many decision making statements that help the flow of the C Sharp program based on certain logical conditions.&#x20;
* These statements are a bunch of code that can be executed by decision statements and that returns a Boolean expression that is true or false.&#x20;
* If the condition is true, it will return true, if the condition is false, it will return false. This Boolean expression generates the Boolean value which could be either true or false.

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

## Types of Conditional Statements

Specific statements to control the flow based on the conditions, we can use&#x20;

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

* if statement.
* if-else statement.
* if-else-if - Or a nested if-else statement that is also known as ladder statement.
* Switch statement - Switch statement is basically used for menu driven applications. we use switch case for menu drivin application.

### Switch Case Code

```csharp
switch (result)
{
    case ("logged in"):
        Console.WriteLine("You are in control");
        break;

    case ("logged out"):
        Console.WriteLine("You do not have access");
        break;

    default:
        Console.WriteLine("Denied");
        break;
}
```

<mark style="color:orange;">Why do we write break after each case?</mark>&#x20;

Let's say our admin userType case match. So after printing this statement, it will also come to the next case and print. We really don't want to do this. We really want to break or go out of this switch case once this condition is satisfied or this block of code is executed.
