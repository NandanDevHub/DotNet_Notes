# C# Code Execution & Basics

## C# Code Execution Process

* C-sharp is a very general purpose, strongly type lexically scoped, object-oriented and component oriented programming language.&#x20;
* Whenever we write any C-Sharp code, there are some steps of process gets executed to compile your code.&#x20;
* Whenever we write any C-sharp program, the program is compiled using C-Sharp compiler that is known as a <mark style="background-color:purple;">C# compiler</mark> also. At this stage, compiler checks if the code contains an error or not.
* If no error is found, then the compiler move to the next step or if compiler founds the error, then it will immediately tell the developer that an error is found in the given line so that the developer can correct them.&#x20;
* After correcting the error, when you run the code, the compiler again checks for the errors. If there are no errors found. It comes to this second step.&#x20;

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Series of Steps of Execution</p></figcaption></figure>

* During this process of intermediate code, what gets happen is <mark style="background-color:purple;">The code gets converted into the intermediate programming language,</mark> which is known as NCIL or IL, which is intermediate language code.&#x20;
* <mark style="color:orange;background-color:orange;">This IL code can run on any operating system because C-sharp is a platform independent language. After converting the C-Sharp source code to common intermediate language or intermediate language code, C-sharp uses the dotnet framework and use as a part of dotnet framework virtual machine component to manage the execution.</mark>&#x20;
* That is what the JIT comes into the picture. The process of JIT tells the machine to use this native language to understand by the machines and execute the code.&#x20;
* During that process, the code gets converted into the dot EXE or dot DLL file, which is an executable piece of code that needs to be executed.&#x20;
* An EXE file represents a program that can be executed and a DLL file includes libraries that can be reused across the different platforms.&#x20;
* This is something how the whole process of compilation and execution of C-Sharp code takes place.
