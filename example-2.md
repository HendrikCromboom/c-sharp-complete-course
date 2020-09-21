```
var fibonacciNumbers = new List<int> {1, 1};
int fibMax = 1836311903;

for(int i=0; fibonacciNumbers[fibonacciNumbers.Count -1] < fibMax; i++){
var previous = fibonacciNumbers[fibonacciNumbers.Count - 1];
var previous2 = fibonacciNumbers[fibonacciNumbers.Count - 2];
fibonacciNumbers.Add(previous + previous2);
}

foreach(var item in fibonacciNumbers)
    Console.WriteLine(item);
```

[Back to Index](index.md) |[Back to Lists](lists.md)