# Property

<figure><img src="../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>

* Internally, C Sharp **properties** are special methods. Or I should say it is used to assign and read the value from a field as a <mark style="background-color:blue;">special method by using accessors.</mark> Thus, it has two accessor, a get property accessor or a getter, and a set property accessor or a setter.
* Unlike fields, properties do not denote storage locations and you cannot pass a property as a ref or a parameter into the functions.

<figure><img src="../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

We can have logic while setting the values in C Sharp that is considered as putting on the validations.

We can make fields of a class private so that fields can't be accessed from outside the class directly thus the property would be needed. Property also need to log all access for a field, and it helps to protect a field by reading and writing.

<figure><img src="../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

### Type of the properties &#x20;

1. Read-write property allows you to assign and read the value of a field. To create a read-write property, we should define get and set, both accessors. We have a read-only property too.&#x20;
2. The read-only property allows you to only retrieve the value of a field, thus, only accessor get is required.&#x20;
3. Write-only property allows you to only change the value of the field thus set property or a set accessor is required. I
4. In the case of auto implemented property, this property is introduced since C Sharp 3.0. Unlike standard property, it is auto implemented property wrapped or backing field is automatically created by compiler. You do not need to take a stress, but we should use this auto implemented property when you do not insisted or required to use the conditions or putting up the validations on a particular field

<mark style="background-color:orange;">Always start the property name with Capital Letter</mark>



#### Getter & Settter

```csharp
		private string name;
		private string companyName;
		private int age;

// Constructor
		public User()
		{
			companyName = "Emerson";
		}
		
// Getter and Setter Property

		public string Name
		{
			get { return name; }
			set { name = value; }
		}
		
// Only Getter Property
		public string CompanyName
		{
			get { return companyName; }
		}
		
// Auto Implemented Property
		private string City { get; set; }
```

### Auto Implemented Property

Let's say **City** we set get and set at the same time you can just write, get and set. <mark style="color:purple;">The property is known as auto implemented property.</mark> This property will exactly behave like this name property which has a getter and setter. You can first set the value and then you can later get the value.

This really helps you in the larger application, especially in the case of MVC, ASP. NET MVC core, where we would like to make a auto implemented model class or a user domain.

