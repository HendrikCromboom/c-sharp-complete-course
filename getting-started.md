# Getting Started

### Install IDE

C#/C-Sharp can be written in any text document or IDE, but I highly advice you to install an IDE that is tailored to .NET.
This will allow you to do a variety things that are specific to a general-purpose, multi-paradigm programming language such as C#. Some examples are creating packages and builds, injecting .NET Core dependencies, run previews and much, much more.

I personally use [Rider](https://www.jetbrains.com/rider/) but there are many other free and premium IDE's out there. 

For an in-debt guide on installing Rider on any system: [Start Here](https://www.jetbrains.com/help/rider/Installation_guide.html#snap).

For the Linux users out there the following [guide](https://sourcedigit.com/20839-extract-install-tar-gz-files-ubuntu/) will explain how to install tar-gz packages.

---

### Install a recent .NET Core build

In order to run anything in .NET we have to have the .NET Core on our OS, this usually isn't deployed out of the box on most OS. 

The following [documentation](https://docs.microsoft.com/en-us/dotnet/core/install/) can be used to install and troubleshoot .NET Core.

You can check your current version in the console `dotnet --version`

OR

In Rider go to File > Settings > Environment.

---

### Install Compiler

* Windows: 

The .NET framework has csc included and will be be able to compile out of the box using the following command in the directory of your C# build:

`csc /out:program_name.exe source_file.cs`

We will get back to the meaning of these parameters when we create our first "Hello World!"

* Linux/Mac:

For Unix/Linux we need to install Mono first:

`sudo apt-get update`

`sudo apt-get install mono-complete`

To compile a file:

`mcs -out:hello.exe hello.cs`

Again, we will cover compiling later

---

[Back to Index](README.md) |[Next](hello-world.md)


