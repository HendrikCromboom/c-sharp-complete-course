# Hello World!

### Setting up a solution

* Let's start off by creating a new solution in the IDE(for a step by step guide we assume you use Rider):

* File > New... > Console Application

* Set the language to C# and change the Solution name > press create.

### Your first piece of code

* The IDE might already use a template to create your very first "Hello World", if it doesnt paste the following code in the empty .cs file:

```
using System;

namespace Hello_World_Console
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

* As you can see `Console.WriteLine("Insert Text")` is the command that outputs text in the console.

* Let's not worry about the rest of the code just yet.

### Running the code in Rider

* In your IDE on the top bar: Run > Run... > "Name of your solution"

* On the bottom we can now see the code getting executed! Eureka!

### Running the code in console

* In your terminal/dash/console line go to the directory where your solution is stored and type the following to compile to an executable file:

`mcs -out:desiredfilename.exe nameofyourcsfile.cs`

* To run the file:

`mono desiredfilename.exe`

---

[Back to Index](index.md) |[Next](the-basics.md)

 
