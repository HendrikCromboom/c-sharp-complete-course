# The Basics

### Strings

* A string is a line of text that can be displayed:

`Console.WriteLine("Hello Hendrik!");`

* "Hello World" is a string, it starts and ends with "double quotes".

* In many other languages both 'single' and "double" quotes can be used to define strings, in Csharp a single quote defines a character.

```
char c = 'c';           //This is a Character
string s = "s";         // This is a String containing a single Character.
```
* In the Hello World program we made edit the string "Hello World", so it displays your name instead of world.

### Variables

* Variables hold values that you can use in the rest of your code:

```
var name = "Name";
Console.WriteLine("Hello " + name + "!");
```

* Edit your code, so the variable contains your name and print it in the console.

* Another way to do this would be:

`Console.WriteLine($"Hello {Name}!");`

* This is what we call String Interpolation and it can make your code quite a bit more concise

* Everything after the "$' will be considered part of the string and you can put variables inside of {brackets}.

* Feel free to try this method as well if you prefer to type less, it's nice to already get a hang of Interpolation

### Methods

* Methods are little workers that take an input and return a result after doing their action

`Console.WriteLine($"Hello {name.ToUpper()}!");`

* In the example above the `ToUpper` method is used to turn the string into ALL CAPS. Methods are always behind the thing you want to alter and start with a `.`

* You know what to do: Get shouting!

### Collections

* Collections are to nobodies surprise a collection of values with the same type.

* For those who have worked in different languages collections might remind them of arrays, yet a bit more complex:

```
var names = new List<string> { "Hendrik", "Felipe", "Emillia" };
foreach (var name in names)
{
    Console.WriteLine($"Hello {name.ToUpper()}!");
}
```

* The variable names will now be a Collection of Strings

* The foreach loop is used to print every string in the collection, no need to worry about what loops are just yet...

* Try creating a collection and copy-paste the foreach loop to print all the strings

---

[Back to Index](index.md) |[Next](numbers.md)