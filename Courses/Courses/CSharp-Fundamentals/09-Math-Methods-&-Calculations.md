# 📐 Math Methods & Calculations

## The "Math" Class

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unlocking the power of the "Math" class in C#. Get ready to add some mathematical magic to your code! 🎓🔢✨

[Slide 1: Introducing the "Math" Class]
- ➡️ Enter the world of numbers with the "Math" class! In C#, this class is a treasure trove of mathematical functions, providing a wide array of operations.

[Slide 2: Common Mathematical Functions]
- 🧮 Let's explore some common functions offered by the "Math" class:
  - **`Math.Abs(x)`**: Returns the absolute value of x.
  - **`Math.Sqrt(x)`**: Returns the square root of x.
  - **`Math.Pow(x, y)`**: Returns x raised to the power of y.
  - **`Math.Round(x)`**: Rounds x to the nearest integer.

[Slide 3: Examples - Absolute Value]
- ➕➖ The absolute value wonder! Let's see how to use `Math.Abs(x)` to get the absolute value of a number.
```csharp
int number = -5;
int absoluteValue = Math.Abs(number);
Console.WriteLine($"Absolute value of {number} is {absoluteValue}");
```

[Slide 4: Examples - Square Root]
- √ The root of the matter! Calculate the square root using `Math.Sqrt(x)`.
```csharp
double number = 25;
double squareRoot = Math.Sqrt(number);
Console.WriteLine($"Square root of {number} is {squareRoot}");
```

[Slide 5: Examples - Power]
- 🚀 Power up with `Math.Pow(x, y)`! Raise a number to a power.
```csharp
double baseNumber = 2;
double exponent = 3;
double result = Math.Pow(baseNumber, exponent);
Console.WriteLine($"{baseNumber} raised to the power of {exponent} is {result}");
```

[Slide 6: Examples - Rounding]
- 🔄 Round and round we go! Utilize `Math.Round(x)` to round a floating-point number.
```csharp
double originalNumber = 3.75;
double roundedNumber = Math.Round(originalNumber);
Console.WriteLine($"Rounded value of {originalNumber} is {roundedNumber}");
```

[Slide 7: Constants in "Math" Class]
- 🔐 The constants corner! The "Math" class also provides useful constants:
  - **`Math.PI`**: The mathematical constant π.
  - **`Math.E`**: The mathematical constant e.

[Slide 8: Examples - Constants]
- 🥧📏 Embrace the constants! Use `Math.PI` and `Math.E` in your calculations.
```csharp
double circleRadius = 5;
double circleArea = Math.PI * Math.Pow(circleRadius, 2);
Console.WriteLine($"Area of the circle with radius {circleRadius} is {circleArea}");

double exponentialValue = Math.Pow(Math.E, 2);
Console.WriteLine($"e raised to the power of 2 is {exponentialValue}");
```

[Slide 9: Benefits of "Math" Class]
- 🌐 Beyond arithmetic! The "Math" class elevates your mathematical capabilities in C#, making complex calculations a breeze.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've harnessed the power of the "Math" class in C#. Today, we explored common functions, constants, and applied them in practical examples. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a math magician in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep calculating with the "Math" class! 🎉🔢✨

## Max Method

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the world of finding the maximum value with the `Max` method in C#. Get ready to explore the peaks of your data! 📈🔝✨

[Slide 1: Unveiling the `Max` Method]
- ➡️ Meet the "Max" method! In C#, the `Max` method is part of the LINQ (Language Integrated Query) library, allowing us to easily find the maximum value in a collection.

[Slide 2: Common Usage of `Max`]
- 📈 Finding the summit! The `Max` method is commonly used with collections of numbers to identify the highest value.

[Slide 3: Syntax of `Max`]
- 📝 Let's break down the syntax of the `Max` method:
  - **`Enumerable.Max<TSource>(IEnumerable<TSource> source)`**: Returns the maximum value in the source collection.

[Slide 4: Example - Finding the Max]
- 🔍 Let's see it in action! Suppose we have an array of numbers, and we want to find the maximum value using the `Max` method.
```csharp
int[] numbers = { 7, 15, 3, 22, 9 };
int maxValue = numbers.Max();
Console.WriteLine($"The maximum value is: {maxValue}");
```

[Slide 5: Example - Finding the Max in a List]
- 📊 Collections of possibilities! The `Max` method works with various collection types. Let's use a List in this example.
```csharp
List<double> scores = new List<double> { 92.5, 88.3, 96.7, 90.1, 94.8 };
double highestScore = scores.Max();
Console.WriteLine($"The highest score is: {highestScore}");
```

[Slide 6: Handling Empty Collections]
- 🛑 A cautious climb! When using `Max`, be mindful of empty collections. It's a good practice to check if the collection has elements before invoking the method to avoid runtime exceptions.

[Slide 7: Example - Handling Empty Collections]
- 🚧 Safeguarding the climb! Check if the collection has elements before attempting to find the maximum.
```csharp
List<int> emptyList = new List<int>();
int maxInEmptyList = emptyList.Any() ? emptyList.Max() : 0;
Console.WriteLine($"The maximum value in the empty list is: {maxInEmptyList}");
```

[Slide 8: Benefits of `Max`]
- 🏔️ Reaching new heights! The `Max` method simplifies the process of finding the maximum value, making your code more concise and readable.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've conquered the peaks with the `Max` method in C#. Today, we explored its syntax, examples, and considerations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a summit seeker with the `Max` method in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep reaching for the max! 🎉🔝✨

## Min Method

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're delving into the world of finding the minimum value with the `Min` method in C#. Get ready to explore the valleys of your data! 📉🔍✨

[Slide 1: Unveiling the `Min` Method]
- ➡️ Enter the "Min" method! Just like its counterpart, the `Min` method is part of the LINQ (Language Integrated Query) library, enabling us to effortlessly find the minimum value in a collection.

[Slide 2: Common Usage of `Min`]
- 📉 Descending into the depths! The `Min` method is commonly used with collections of numbers to identify the lowest value.

[Slide 3: Syntax of `Min`]
- 📝 Let's dissect the syntax of the `Min` method:
  - **`Enumerable.Min<TSource>(IEnumerable<TSource> source)`**: Returns the minimum value in the source collection.

[Slide 4: Example - Finding the Min]
- 🔍 Let's put it to the test! Imagine we have an array of numbers, and we want to find the minimum value using the `Min` method.
```csharp
int[] numbers = { 7, 15, 3, 22, 9 };
int minValue = numbers.Min();
Console.WriteLine($"The minimum value is: {minValue}");
```

[Slide 5: Example - Finding the Min in a List]
- 📊 Collections of possibilities! The `Min` method seamlessly works with various collection types. Let's use a List in this example.
```csharp
List<double> temperatures = new List<double> { 24.5, 22.1, 18.8, 20.5, 23.2 };
double lowestTemperature = temperatures.Min();
Console.WriteLine($"The lowest temperature is: {lowestTemperature}");
```

[Slide 6: Handling Empty Collections]
- 🛑 A cautious descent! Similar to `Max`, when using `Min`, be cautious with empty collections. Check if the collection has elements to avoid runtime exceptions.

[Slide 7: Example - Handling Empty Collections]
- 🚧 Safeguarding the descent! Ensure the collection has elements before attempting to find the minimum.
```csharp
List<int> emptyList = new List<int>();
int minInEmptyList = emptyList.Any() ? emptyList.Min() : 0;
Console.WriteLine($"The minimum value in the empty list is: {minInEmptyList}");
```

[Slide 8: Benefits of `Min`]
- 🏞️ Descending to new depths! The `Min` method simplifies the process of finding the minimum value, making your code concise and easy to understand.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've navigated the valleys with the `Min` method in C#. Today, we explored its syntax, examples, and considerations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a valley explorer with the `Min` method in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep searching for the min! 🎉🔍✨

## 📏 Absolute Value

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unraveling the concept of absolute value in C#. Get ready to dive into the world of numbers and magnitudes! ➕➖🔍✨

[Slide 1: Understanding Absolute Value]
- ➡️ What's absolute value? In mathematics, the absolute value of a number is its distance from zero on the number line, regardless of direction. In C#, we use the `Math.Abs` method to find this numerical magnitude.

[Slide 2: Syntax of `Math.Abs`]
- 📝 Let's dive into the syntax of `Math.Abs`:
  - **`Math.Abs(x)`**: Returns the absolute value of x.

[Slide 3: Example - Finding Absolute Value]
- 🔍 Let's bring it to life! Suppose we have a number, and we want to find its absolute value using `Math.Abs`.
```csharp
int number = -7;
int absoluteValue = Math.Abs(number);
Console.WriteLine($"The absolute value of {number} is: {absoluteValue}");
```

[Slide 4: Dealing with Negative Values]
- ➕➖ Handling negativity! Absolute value is especially handy when dealing with negative numbers. It provides a clear, positive representation of the number's magnitude.

[Slide 5: Example - Handling Negative Values]
- 📉 Turning negatives positive! Demonstrate the power of `Math.Abs` with a negative number.
```csharp
int negativeNumber = -15;
int positiveMagnitude = Math.Abs(negativeNumber);
Console.WriteLine($"The absolute value of {negativeNumber} is: {positiveMagnitude}");
```

[Slide 6: Use Cases in Real-world Scenarios]
- 🌐 Real-world applications! Absolute value is crucial in various scenarios, such as calculating differences, distances, or ensuring non-negative values.

[Slide 7: Example - Calculating Differences]
- 📊 Bridging differences! Calculate the absolute difference between two numbers.
```csharp
int num1 = 25;
int num2 = 18;
int absoluteDifference = Math.Abs(num1 - num2);
Console.WriteLine($"The absolute difference between {num1} and {num2} is: {absoluteDifference}");
```

[Slide 8: Benefits of Absolute Value]
- 🌈 Beyond numbers! Absolute value brings clarity to numerical magnitudes, making your code more robust and adaptable to various scenarios.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've mastered the art of absolute value in C#. Today, we explored its syntax, examples, and real-world applications. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a magnitude maestro with absolute value in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep exploring the world of numbers! 🎉➕➖✨

In mathematics, the absolute value or modulus of a real number is the non-negative value of the number without regard to its sign.

It is denoted by `|x|`, where `x` is a real number.

Example `3.1`:

```csharp
var x = int.Parse(Console.ReadLine());

var absoluteValue = Math.Abs(x);
Console.WriteLine(absoluteValue);
```

The `Math.Abs()` method returns the non-negative value of `x`.

The absolute value of a number measures the distance of the number from zero along the real number line, regardless of its direction, and is always a positive value.

Normally, we would use such functions when working with the value itself, regardless of its sign.

Example `3.2`:

```csharp
var x = int.Parse(Console.ReadLine()); // Example: "-5"

//                               👇 -(-5) = 5
var absoluteValue = x >= 0 ? x : -x;
Console.WriteLine(absoluteValue); // 👈 Prints "5"
```

Examples `3.1` and `3.2` are logically equivalent.

## Raise To Power

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unlocking the power of exponentiation in C#. Get ready to elevate your numbers to new heights! 🚀🔢✨

[Slide 1: Understanding Exponentiation]
- ➡️ What is exponentiation? In mathematics, exponentiation is the process of raising a number to a specific power. In C#, we use the `Math.Pow` method to achieve this mathematical marvel.

[Slide 2: Syntax of `Math.Pow`]
- 📝 Let's delve into the syntax of `Math.Pow`:
  - **`Math.Pow(x, y)`**: Returns x raised to the power of y.

[Slide 3: Example - Raising to Power]
- 🔍 Let's put it into action! Suppose we have a base number, and we want to raise it to a power using `Math.Pow`.
```csharp
double baseNumber = 2;
int exponent = 3;
double result = Math.Pow(baseNumber, exponent);
Console.WriteLine($"{baseNumber} raised to the power of {exponent} is: {result}");
```

[Slide 4: Exponentiation in Real-world Scenarios]
- 🌐 Real-world applications! Exponentiation is not just a mathematical concept; it finds applications in various fields, such as compound interest calculations, growth projections, and more.

[Slide 5: Example - Compound Interest]
- 📈 Growing wealth! Showcase the application of exponentiation in compound interest calculations.
```csharp
double principal = 1000;
double rate = 0.05;
int years = 3;
double compoundInterest = principal * Math.Pow(1 + rate, years);
Console.WriteLine($"After {years} years, the compound interest is: {compoundInterest}");
```

[Slide 6: Handling Negative Exponents]
- ➖ Handling the negative! Exponentiation is versatile; it can handle negative exponents, resulting in fractions or decimals.

[Slide 7: Example - Negative Exponent]
- ➖ Turning the power around! Illustrate the use of negative exponents in calculations.
```csharp
double baseNumber = 3;
int negativeExponent = -2;
double result = Math.Pow(baseNumber, negativeExponent);
Console.WriteLine($"{baseNumber} raised to the power of {negativeExponent} is: {result}");
```

[Slide 8: Benefits of Exponentiation]
- 🌟 Empowering numbers! Exponentiation provides a powerful tool for expressing growth, decay, and various mathematical phenomena in a concise and expressive manner.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've harnessed the power of exponentiation in C#. Today, we explored its syntax, examples, and real-world applications. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a mathematical sorcerer, raising numbers to new heights with exponentiation in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep elevating your code! 🎉🔢✨

## Square Root

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unlocking the secrets of square roots in C#. Get ready to dig into the roots of numbers and unveil their mysteries! 🌱🔢✨

[Slide 1: Understanding Square Roots]
- ➡️ What is a square root? In mathematics, the square root of a number is a value that, when multiplied by itself, gives the original number. In C#, we use the `Math.Sqrt` method to find this mystical value.

[Slide 2: Syntax of `Math.Sqrt`]
- 📝 Let's dive into the syntax of `Math.Sqrt`:
  - **`Math.Sqrt(x)`**: Returns the square root of x.

[Slide 3: Example - Finding Square Root]
- 🔍 Let's bring it to life! Suppose we have a number, and we want to find its square root using `Math.Sqrt`.
```csharp
double number = 9;
double squareRoot = Math.Sqrt(number);
Console.WriteLine($"The square root of {number} is: {squareRoot}");
```

[Slide 4: Handling Negative Numbers]
- ➖ Negative roots! While square roots of negative numbers are not real in the realm of real numbers, C# handles them using the `NaN` (Not a Number) result.

[Slide 5: Example - Handling Negative Numbers]
- ➖ Navigating the imaginary! Illustrate the result of trying to find the square root of a negative number.
```csharp
double negativeNumber = -4;
double result = Math.Sqrt(negativeNumber);
Console.WriteLine($"The square root of {negativeNumber} is: {result}");
```

[Slide 6: Square Roots in Real-world Scenarios]
- 🌐 Real-world applications! Square roots find applications in various fields, such as physics, engineering, and statistics, where the magnitude of values is essential.

[Slide 7: Example - Calculating Distance]
- 📏 Measuring distance! Showcase the application of square roots in calculating distances.
```csharp
double x1 = 1;
double y1 = 2;
double x2 = 4;
double y2 = 6;
double distance = Math.Sqrt(Math.Pow(x2 - x1, 2) + Math.Pow(y2 - y1, 2));
Console.WriteLine($"The distance between the points is: {distance}");
```

[Slide 8: Benefits of Square Roots]
- 🌱 Rooting for clarity! Square roots help us understand the magnitudes of numbers, aiding in precise measurements and calculations.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've uncovered the secrets of square roots in C#. Today, we explored its syntax, examples, and real-world applications. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a number whisperer, unraveling the mysteries of square roots in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep digging into the roots of your code! 🎉🔢✨

## Rounding Numbers

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the world of rounding numbers in C#. Get ready to make your numbers sleek and precise! 🔄🔢✨

[Slide 1: Why Round Numbers?]
- ➡️ Why round numbers? Rounding is crucial to simplify and present numbers in a more manageable form, especially when dealing with real-world scenarios that require precision.

[Slide 2: Common Rounding Methods]
- 🔄 Let's explore the common rounding methods:
  - **Round**: Rounds to the nearest whole number.
  - **Ceiling**: Rounds up to the nearest whole number.
  - **Floor**: Rounds down to the nearest whole number.

[Slide 3: Example - Rounding to the Nearest Whole Number]
- 🔍 Let's round it up! Suppose we have a decimal number, and we want to round it to the nearest whole number using `Math.Round`.
```csharp
double decimalNumber = 7.8;
int roundedNumber = (int)Math.Round(decimalNumber);
Console.WriteLine($"Rounded number: {roundedNumber}");
```

[Slide 4: Example - Rounding Up]
- 🚀 Up, up, and away! Use `Math.Ceiling` to round a decimal number up to the nearest whole number.
```csharp
double decimalNumber = 3.2;
int roundedUpNumber = (int)Math.Ceiling(decimalNumber);
Console.WriteLine($"Rounded up number: {roundedUpNumber}");
```

[Slide 5: Example - Rounding Down]
- 📉 Heading down! Utilize `Math.Floor` to round a decimal number down to the nearest whole number.
```csharp
double decimalNumber = 9.7;
int roundedDownNumber = (int)Math.Floor(decimalNumber);
Console.WriteLine($"Rounded down number: {roundedDownNumber}");
```

[Slide 6: Rounding with Precision]
- 🎯 Precision matters! Rounding can also be performed with a specific number of decimal places using the `Math.Round` method with a second parameter.

[Slide 7: Example - Rounding with Precision]
- 🎯 Pinpoint precision! Demonstrate rounding a decimal number to a specific number of decimal places.
```csharp
double decimalNumber = 5.6789;
double roundedWithPrecision = Math.Round(decimalNumber, 2);
Console.WriteLine($"Rounded with precision: {roundedWithPrecision}");
```

[Slide 8: Benefits of Rounding]
- 🌈 Rounding for clarity! Precision in numbers is essential for readability and conveying information accurately.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've mastered the art of rounding numbers in C#. Today, we explored rounding to the nearest whole number, rounding up, rounding down, and precision rounding. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a number sculptor, shaping your numbers with precision in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep your numbers sleek and rounded! 🎉🔄✨