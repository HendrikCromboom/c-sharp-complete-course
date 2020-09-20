# Numbers

### Integers

* Integers are whole numbers, both positive and negatives.

* Csharp uses the basic mathematical rules of priority calculation:
```
int a = 5;
int b = 4;
int c = 2;
int d = (a + b) - 6 * c + (12 * 4) / 3 + 12;
Console.WriteLine(d);
```

* Notice that if a calculation of integers does not result in a whole number, it will get rounded down.

### Doubles

* Doubles are double-precision floating point numbers.

* Floating point means that they are non integral numbers with a large min and max value.

* Double-precision means that the numbers have twice the number of binary digits, this allows for tracking of decimals for example.

```
double a = 5;
double b = 4;
double c = 2;
double d = (a + b) / c;
Console.WriteLine(d);
```

* As you can see the decimals are retained with doubles.

### Decimals

* While decimals do not have the same range as doubles, they have great precision:

```
double a = 1.0;
double b = 3.0;
Console.WriteLine(a / b);

decimal c = 1.0M;
decimal d = 3.0M;
Console.WriteLine(c / d);
```

* As you can see we can track the decimals to am extensive degree.

* The suffix M allows us to define that the constant is a decimal, if we don't the compiler will assign the double type to it.

### Math Field

* In .NET Core 3.1 we have 2 math fields that can be used for calculations

    * Math.PI (PI is used for calculations of circles and angles)
    * Math.E (E is used for logarithmic comparing, and represents the natural logarithmic base)
    
* Both are used in some edge cases of web development but are mostly useful for engineers, game designers,...

* Just remember that if you ever require to calculate the surface of a circle, there is a field that can make this easier for you

### Math Methods

* At this point we should be able to do calculations with +,-,* and /

* .NET Core 3.1 has an entire range of complex of methods that can simplify a lot of work for you

* Again there are some edge cases in web development, but these methods are mostly useful for system operations, engineering,...

* Just remember that you can always look at the [Documentation](https://docs.microsoft.com/en-us/dotnet/api/system.math?view=netcore-3.1)

### Conclusion

* There are 3 common types of numbers in Csharp: integrals, doubles and decimals.

* If we do not keep these different types in mind, we might end up with calculation results that are not in line with our expectations because Csharp is a strong-typed language.

* A strong-typed language will not compile if the required type is not specified, throw an error during compilation if it's implicated as wrong or default to an expected type on compilation. (Remember the example with Decimals if we don't specify M?)

---

[Back to Index](README.md) |[Next](next.md)

    


