# Console

### WriteLine

* By now if you have used the terminal to test some of your scripts you should have noticed that `Console.WriteLine()` outputs directly into the terminal when we create a terminal/console application.

* While it might not be in our best interest, we can put entire functions inside the WriteLine.

```
int a = 1;
int b = 2;
Console.WriteLine((a+b)/2)
```

### ReadLine

* WriteLine and ReadLine are one of the most famous duos ever, the first one prints something in the console, the second fetches the users response.

```
Console.WriteLine("Would you like a cake? (Y/N)?")
var yesOrNo = Console.ReadLine()
```

* If Read and Write are combined we can use them as a question and answer event, just like the example above


### Clear

* `Console.Clear() clears the entire console, didn't see that one coming did you? I know consider my mind equally blown...`

### And so much more

* The console  has tons of features, while the documentation might be overwhelming you could brick your brain [Here!](https://docs.microsoft.com/en-us/dotnet/api/system.console?view=netcore-3.1)

* In the upcoming chapters we might use some of the Console's features, when we do I will refer to them individually, so there is no need to study the above documentation, it's just there for thoroughness's sake...

 [Back to Index](index.md) |[Next](final.md)
