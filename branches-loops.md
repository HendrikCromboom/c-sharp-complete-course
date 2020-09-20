# Branches and Loops

### If statement

* The if statement is used to execute a piece of code "if" a certain statement is "true"

```
int a = 5;
int b = 6;
if (a + b > 10) 
    Console.WriteLine("The answer is greater than 10.");
```

* If the sum of a and b is greater than 10 we will get a console log!

### Boolean

* When we specify a variable to be "true" or "false" we call it a boolean or bool

* In the case of an "if" statement we execute the code after the statement if "bool" is "true"

### Else statement

* If we want to branch out if the "bool" of an "if" statement is "false", we use the "else" statement.

```
int a = 5;
int b = 3;
if (a + b > 10)
    Console.WriteLine("The answer is greater than 10");
else
    Console.WriteLine("The answer is smaller than 10");
```

* If the sum is greater than the console will log "The answer is greater than 10", if it isn't greater than 10 the console will log "The answer is smaller than 10"

### AND operator

* We have already seen +,-,*,/ and =

* These are commonly called operators, another logical operator is "AND", in Csharp "AND" is defined by "&&"

```
int a = 5;
int b = 3;
int c = 4;
if ((a + b + c > 10) && (a == b))
{
    Console.WriteLine("The answer is greater than 10");
    Console.WriteLine("And the first number is equal to the second");
}
else
{
    Console.WriteLine("The answer is not greater than 10");
    Console.WriteLine("Or the first number is not equal to the second");
}
```

* If BOTH of the statements are "true" we execute the if statement, if either or both return "false" we execute the else statement

### OR statement

* Just like AND/&& we have a logical operator called "OR" defined by "||'

```
int a = 5;
int b = 3;
int c = 4;
if ((a + b + c > 10) || (a == b))
{
    Console.WriteLine("The answer is greater than 10");
    Console.WriteLine("Or the first number is equal to the second");
}
else
{
    Console.WriteLine("The answer is not greater than 10");
    Console.WriteLine("And the first number is not equal to the second");
}
```

* If either or both of the statements are true we execute the if statement, if neither are true we execute the else statement

### Loops

* Loops are one of the most concepts in development of any kind

* A loop is a piece of code that keeps repeating untill or while a certain condition is met

```
int counter = 0;
while (counter < 10)           
{
  Console.WriteLine($"Hello World! The counter is {counter}");         
  counter++;                   
}
```

* While counter is smaller than 10 we execute the following code

    * We console log a certain string
    
    * And we increase the integer counter by 1
    
* Execute the above code to get a clearer understanding of loops.

### Do While

* We have already seen the "while statement'

* A variant of this is the "do while" statement

```
int counter = 0;
do
{
  Console.WriteLine($"Hello World! The counter is {counter}");
  counter++;
} while (counter < 10);
```

* If you execute this piece of code you will see that they do exactly the same, it's just a different way of defining things


### For statement

* For those who want to limit the amount of code they write there is the for statement

* While the result is exactly the same as while and do while, the syntax is shorter

```
for(int counter = 0; counter < 10; counter++)
{
  Console.WriteLine($"Hello World! The counter is {counter}");
}
```

* The first parameter is the initialisation of the variable

* The second part is the "while" part

* The third part usually defines the increment or decrement of the loop

```
for(initializer; condition; iterator)
```

### Loop-ception

* You will quickly realise that we can combine loops to further specify conditions, these are called "Nested Loops"

```
for (int row = 1; row < 11; row++)
{
  for (int column = 1; column < 11; column++)
  {
    Console.WriteLine($"The cell is ({row}, {column})");
  }
}
```

* The code above will iterate over a number of rows from 1 to 10 and for each iteration it will iterate over an amount of columns ranging from 1 to then, for each of the 100 total iterations it will console log the number of row and column it's at.

### Example

* If you want you can try solving this small fizz-buzz variant

```
Find the sum of all integers 1 through 20 that are divisible by 3.
```
* You may need the "%" operand, but there are many solutions for this one

### Solution

* The result should be 63

* You can check one of the many solutions [HERE](example-1.md)


