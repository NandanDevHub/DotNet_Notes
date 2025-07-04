---
description: >-
  .NET CLI is, its advantages, and how it simplifies the development and
  deployment process.
---

# .Net Core Architecture & .Net CLI

## Introduction to .NET CLI

* .NET Core CLI is a new cross-platform tool that is used for creating, restoring packages, building and publishing.NET applications.
* it also supports installation of third-party packages. Basically, when we use Visual Studio for creating the.NET applications, Visual Studio also internally uses the.NET CLI commands to restore, build, and publish the applications.
* It also supports various commands that can be used to create, build, and run.NET Core projects.
* We can also use.NET Core CLI to manage the dependencies, whether to add the third party dependencies, removing them, or updating them using.NET nugget package manager.
* It can be easily automated and integrated into build and deployment pipeline because it supports the command line interface.&#x20;
* When we install.NET Core SDK, then by default.NET Core CLI is also installed. So we don't require installing it separately on the development environment or our local machine.

<figure><img src="../.gitbook/assets/image (117).png" alt=""><figcaption></figcaption></figure>

**To Check wheather .Net CLI is installed in out machine or not**

Upon firing --version check or just not if if returns version or --help options that means .dot net CLI is installed on ou rcomputer.

### .NET CLI Command Structure

```
dotnet <command> <arguement> <option>
```

* All the.NET Core CLI command starts with the driver named <mark style="color:orange;">dotnet</mark>.&#x20;
* The driver <mark style="color:orange;">dotnet</mark> starts to execution of the specific <mark style="color:purple;">command</mark>, we can supply command to perform a specific action.&#x20;
* Each command can be followed by the <mark style="color:purple;">arguments</mark> and <mark style="color:purple;">options</mark><mark style="color:blue;">.</mark>
* For example, <mark style="color:orange;">dotnet</mark> is the driver, then we specify the <mark style="color:purple;">command</mark> _that we wanted to create a new project._ `(new)` \
  <mark style="color:purple;">argument</mark> _that what kind of project you want it to generate_, and then the <mark style="color:purple;">options</mark>, for example, <mark style="color:purple;">the name of the project or other entities that you want it to include into your project</mark> as well.

<figure><img src="../.gitbook/assets/image (118).png" alt=""><figcaption><p>.Net CLI Command Structure</p></figcaption></figure>

## .NET CLI Commands

We can use this command `dotnet-help` to get the list of commands the tool is offering. After that, below commands will get over there. We need to opt out. What are the commands we wanted to execute.

<figure><img src="../.gitbook/assets/image (119).png" alt=""><figcaption><p>.NET CLI Commands</p></figcaption></figure>

#### Advancend & Project Modification CLI Commands

<figure><img src="../.gitbook/assets/image (120).png" alt=""><figcaption><p>Advanced CLI Commands</p></figcaption></figure>

### Demo - Generate a new project with the help of.NET CLI command

```bash
// Creating Project using dotnet CLI

dotnet new list

dotnet new web --name CLIWebProj

dotnet build

dotnet run
```

## Documentation Links

{% embed url="https://learn.microsoft.com/en-us/dotnet/core/tools/" %}
.NET CLI overview
{% endembed %}

{% embed url="https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet?source=recommendations" %}
dotnet command
{% endembed %}
