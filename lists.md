# Lists

### Recap

* In the first lesson we already covered collections quickly:

```
var names = new List<string> { "World", "Ana", "Felipe" };
foreach (var name in names)
{
  Console.WriteLine($"Hello {name.ToUpper()}!");
}
```

* A  List<T> is a type of collection we can store add and remove values from

### Adding and removing values

* We can add values to a list with .Add() method, let's put that in practice:

```
var names = new List<string> { "World", "Ana", "Felipe" };
names.Add("Maria");
names.Add("Bill");
foreach (var name in names)
{
  Console.WriteLine($"Hello {name.ToUpper()}!");
}
```

* When we want to remove items from the list we use .Remove()

```
var names = new List<string> { "World", "Ana", "Felipe", "Maria", "Bill" };
names.Remove("World");
foreach (var name in names)
{
  Console.WriteLine($"Hello {name.ToUpper()}!");
}
```

### Index

* Every item in the list has an index starting with 0, think of them as a way to specify items in a list:

```
var names = new List<string> { "Ana", "Felipe", "Maria", "Bill" };
Console.WriteLine($"Our first item changed to {names[0]}.");
Console.WriteLine($"I've added {names[2]} and {names[3]} to the list.");
```

* As you can see we can use square brackets to call upon a value using its index, for this example [0,1,2,3]

* Another useful method is .Count:

```
var names = new List<string> { "Ana", "Felipe", "Maria", "Bill" };
Console.WriteLine($"The list has {names.Count} people in it");
```

* The Count method will return the amount of values that are in the List, 4 in this case

### Searching lists

* If we want to look for a certain value in a List we can use the .IndexOf() method:

```
var names = new List<string> { "Ana", "Felipe", "Maria", "Bill" };
var index = names.IndexOf("Felipe");
if (index != -1)
  Console.WriteLine($"The name {names[index]} is at index {index}");

var notFound = names.IndexOf("Not Found");
  Console.WriteLine($"When an item is not found, IndexOf returns {notFound}");
```

* When using "IndexOf" the method will look for an exact match in the list and return it's index

* If no match is found, the method will return the value "-1"

* In the example above we use the returned value in an IF ELSE branch to console log if the search was succesful

### Sorting Lists

* When we have large lists it might be useful to sort them:

```
var names = new List<string> { "Ana", "Felipe", "Maria", "Bill" };
names.Sort();
foreach (var name in names)
{
  Console.WriteLine($"Hello {name.ToUpper()}!");
}
```

* The .Sort() method will rearrange the values in the list to alphabetical order if they are strings

### Exercise

* The same way we can create Lists<T> for strings, we can create lists of integers

* For this case lets output all the [Fibonacci Numbers](https://en.wikipedia.org/wiki/Fibonacci_number) in console

* Fibonacci numbers start with [1, 1] and every number after it is the sum of the last 2 numbers, so: [1,1,2,3,5,8,...1836311903]

* You will probably need a loop for this one

* Just so you do not brick your console or potato I will provide you with the largest Fibonacci number C# can calculate from integers: `1836311903`

### Solution

* You can check one of the many solutions [HERE](example-1.md)

* You should have the following output in your console:

`1
 1
 2
 3
 5
 8
 13
 21
 34
 55
 89
 144
 233
 377
 610
 987
 1597
 2584
 4181
 6765
 10946
 17711
 28657
 46368
 75025
 121393
 196418
 317811
 514229
 832040
 1346269
 2178309
 3524578
 5702887
 9227465
 14930352
 24157817
 39088169
 63245986
 102334155
 165580141
 267914296
 433494437
 701408733
 1134903170
 1836311903`
 
 [Back to Index](index.md) |[Next](lists.md)