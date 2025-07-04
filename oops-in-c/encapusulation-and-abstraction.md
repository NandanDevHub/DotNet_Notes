# Encapusulation and Abstraction

## Encapsulation

<mark style="color:purple;">Encapsulation allows the programmer to implement the desired level of abstraction.</mark>&#x20;

In short, it is a <mark style="color:purple;">process of hiding all internal details of an object from outside the world.</mark>&#x20;

We hide the data, making it <mark style="color:yellow;">private</mark> and expose a <mark style="color:yellow;">public</mark> property to <mark style="color:purple;">access those data from outside the world.</mark>&#x20;

Encapsulation can also be considered as data hiding because it helps in implementing the key feature of object-oriented programming that is, a data security or data hiding.&#x20;

Encapsulation can be achieved by declaring all the variables in the class as private that is by default.&#x20;

If you wanted to access it from outside the class definition, you need to abstract the data members and member functions with the help of different other access modifiers.&#x20;

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

Considering this is my student class and these are my data members,&#x20;

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

if I do not write any access modifier in front of them, they are by default private. This is the private and this is the <mark style="color:yellow;">private</mark> data access modifier by default, whether you write it or not.&#x20;

If any of the member is <mark style="color:yellow;">private</mark>, <mark style="background-color:purple;">it means it is encapsulated cannot be accessed from outside the class definition.</mark>&#x20;



<figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

You can see that if I will try to access student.studentId, I cannot access this but if I go to my studentId and I will keep it public, I can easily access this member from outside the class definition.&#x20;

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

It means that if I'm making any of the access modifier as <mark style="color:yellow;">private</mark> for any property or behavior or data member or member function.<mark style="color:orange;">It means I am hiding that data from outside the world.</mark>&#x20;

If I want to access it, I need to expose it then a <mark style="color:yellow;">public</mark> property or <mark style="color:yellow;">public access modifier</mark> will be required, such as public except detail and public display detail then only I can access them from this area, from this program.cs but this is a private property. I cannot access this from the outside-the-class definition.&#x20;

## Abstraction

<mark style="color:orange;">Data abstraction is the property by virtue of which only essential details are exhibited to the user.</mark>&#x20;

For example, if you are going to purchase a car, you will not ask for what color they have painted on their wires or their pipes, the what fabric they've used in their seats.&#x20;

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

You will hardly bother about these features and the details.&#x20;

But you will definitely ask for the color of the car. You will definitely ask for whatever the advanced features are and what are their accessibility.&#x20;

<figure><img src="../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

That is what you understand or you try to get all the details which are essential for you.



Abstraction can be achieved with the help of <mark style="color:green;">abstract classes</mark> or <mark style="color:green;">abstract methods. t</mark>hat defines what details needs to be accessed from the outside of the class definition and what needs to be hidden.&#x20;

Consider a real-life scenario of withdrawing money from ATM. The user only knows that in ATM machine first enter the ATM card, then entered the pin code of the ATM, and then enter amount what she or he wants to withdraw, and at last he or she gets the money.&#x20;

<figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

The user does not know about the inner mechanics of the ATM, of withdrawing money. What are the programming will move, use, the technology they have implemented, and so on.&#x20;

That is what the details that you wanted to see. It means you wanted to abstract the details that hardly bothers to you that is encapsulated.&#x20;

<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

To implement the access modifiers that is helping us in abstraction and encapsulation.&#x20;

## Access Modifies

Access modifier that helps in defining the accessibility from where the data needs to be accessed in the programming, public is not restricted, and private is most restricted.&#x20;

<figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

That's what we have discussed so far but along with that, you have <mark style="color:yellow;">public, private, protected, and internal.</mark>&#x20;

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

Sometimes we do have public, and <mark style="color:yellow;">public-private protected internal</mark> and <mark style="color:yellow;">protected internal.</mark>&#x20;

### Types

* <mark style="background-color:purple;">Public</mark> as I discussed, least restricted. If you define any of the member public, you can access it from anywhere outside the names.&#x20;
* <mark style="background-color:purple;">Private</mark> is accessible within the class, within the body itself.&#x20;
* <mark style="background-color:purple;">Protected</mark> helps in inheritance when the parent class has any member as protected, that member can be accessed from the child classes only and from its own class not from other classes.&#x20;
* An <mark style="background-color:purple;">internal</mark> has most implemented and by default, all the classes are internal. Internal means a class or any member of it is internal can be accessed within its own namespace. In whatever classes you have mentioned in the namespace, but not from outside namespace.&#x20;

but <mark style="color:yellow;">public</mark> access modifier is only restricted place that can also be accessed from the other namespaces as well.&#x20;

The last, as I discussed about, the combination is <mark style="color:yellow;">protected internal.</mark>&#x20;

#### <mark style="background-color:purple;">Protected Internal</mark>&#x20;

<mark style="color:purple;">Protected means inheritance</mark>, <mark style="color:orange;">internal means within the namespace</mark>, within the namespace, <mark style="background-color:yellow;">only in the child classes the members can be accessible.</mark>&#x20;

#### What are the access specifiers and from where they can be accessed public, protected, internal, protected internal, as well as private.

<figure><img src="../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>
