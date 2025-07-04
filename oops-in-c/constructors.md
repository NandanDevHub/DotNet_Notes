# Constructors

A constructor is a special method that is used to <mark style="background-color:purple;">initialize an object of a class</mark> which I earlier demonstrated, When you do not assign any values to the attributes or the data members of a class, by default the default values are assigned to them with the help of the <mark style="color:orange;">default constructor</mark> of the object class.&#x20;

But we can also create our own constructor in a specific class. It is similar to other methods that we invoke when an object of a class is created but it has a d\`ifferent behavior.&#x20;

The <mark style="color:purple;">name of the constructor is same as that of the class name</mark> as well as constructors do not have return types.&#x20;

<figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

## Types of Constructors

We have different types of constructors to be implemented defining their different functionalities&#x20;

<figure><img src="../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

If I'm not assigning any values to the studentid and student name.&#x20;

<figure><img src="../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>

The moment I will call this displaydetail with the help of this program CS that is going to display the default values of a specific data type. So you can see that studentid will be 0 and the student's name will be null.&#x20;

Because each and every class is <mark style="color:red;">inherited with the object class in C Sharp</mark> as well as in other programming languages. So when you do not assign any values to the data member, every data type has a specific value to be assigned integer will assign with the default value 0, string with null, float with 0.0, boolean with false and so on.&#x20;

<img src="../.gitbook/assets/file.excalidraw (3).svg" alt="" class="gitbook-drawing">

But if you don't want to assign these default values, you don't want to rely on this <mark style="background-color:red;">object</mark> class. It is completely your choice to write this inheritance or not, but it is implicitly happens.&#x20;

### Default Constructor

You can also define your own default constructor in your class. As I said, the name of the constructor is same as that of the class name that is student and it does not has a return type.&#x20;

```csharp
//Default Constructors
public Student()
{
    studentId = 10;
    studentName = "Annoynomus";
}
```

<mark style="color:purple;">It helps in assigning the default values. As constructor is a special method that even don't need to invoke.</mark> For example, above you are invoking your display detail but constructors are invoked implicitly.

&#x20;For example, this is the area,&#x20;

```
Student student = new Student()
```

this is the place where you are creating an object of a class implicitly. <mark style="color:orange;">This is the constructor instantiation and the constructor gets invoked at this point,</mark> <mark style="color:orange;">you don't need to invoke it separately.</mark> So thus the student constructor default constructor invoked, assigning the default values with the help of this reference variable (student) and that is what the display detail is going to print.&#x20;

So you can see that studentid is 10 one and student name is anonymous.&#x20;

### Parameterized Constructor

Constructor a class can have default constructor as well as other constructor.&#x20;

Lets create a parameterized constructor where I'm saying that there would be a constructor student that will take two values integer studentid, that is sid and sName.&#x20;

```csharp
//Parameterized Constructor
public Student(int sid, string sName)
{
    studentId = sid;
    studentName = sName;
}
```

I'm saying that these parameters needs to be assigned in the studentid I would like to assign sid and in student name I would like to assign sName.&#x20;

So it means that if I will be instantiating a particular object of this particular class let's say&#x20;

```csharp
// Parameterized Constructor
Student parameterizedStudent = new(107, "Rahul");
parameterizedStudent.displayDetails();
```

&#x20;So when I am not passing anything it will always call the default constructor.&#x20;

Let's say first is the integer sid and this is the sName. The moment here the constructor is invoked it will invoke the parameterized constructor assign the sid into the studentid i.e 107 and sName into the student name.  i.e. Rahul , and the time when with the same reference variable I'll call the display detail whatever values you have assigned that gets assigned and printed as well.&#x20;

<mark style="background-color:orange;">Thus more than one constructor can be created into one class and that concept is known as constructor overloading.</mark>&#x20;

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>
