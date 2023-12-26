# 🔃 Control Flow - Loops

## Repeated Actions

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the fascinating world of "Repeated Actions" in C#—a crucial concept achieved through loops. Get ready to unleash the power of iteration and make your code dance! 🔄🕺🔍

[Slide 1: The Need for Repeated Actions]
- ➡️ Often, we encounter scenarios where a certain action needs to be performed multiple times. Loops provide an elegant solution, allowing you to repeat code and automate tasks efficiently.

[Slide 2: The Basics of Loops]
- 🔄 The maestros of repetition! Loops in C# come in various forms, such as the for loop, while loop, and do-while loop. They share the common goal of executing a block of code multiple times.

[Slide 3: The For Loop]
- 🔢 The counting loop! The for loop is ideal when you know the number of iterations in advance.
```csharp
for (int i = 0; i < 5; i++)
{
    // Code to repeat five times
    Console.WriteLine($"Iteration {i + 1}");
}
```

[Slide 4: The While Loop]
- 🔄 The conditional dancer! The while loop repeats as long as a specified condition is true.
```csharp
int counter = 0;
while (counter < 5)
{
    // Code to repeat five times
    Console.WriteLine($"Iteration {counter + 1}");
    counter++;
}
```

[Slide 5: The Do-While Loop]
- 🔄🔍 The persistent performer! The do-while loop guarantees at least one execution, as it checks the condition after the first iteration.
```csharp
int count = 0;
do
{
    // Code to repeat at least once
    Console.WriteLine($"Iteration {count + 1}");
    count++;
} while (count < 5);
```

[Slide 6: Common Loop Practices]
- 🔄🔁 The loop choreography! Loops often involve iterating over collections like arrays or lists, processing elements one by one.

[Slide 7: Breaking Out of Loops]
- ⛔ The escape artist! The `break` statement allows you to exit a loop prematurely, based on a certain condition.

[Slide 8: Skipping Iterations with Continue]
- ⏭️ The dance skipper! The `continue` statement skips the rest of the current iteration and moves to the next one.
```csharp
for (int i = 0; i < 5; i++)
{
    if (i == 2)
    {
        // Skip the rest of iteration 2
        continue;
    }
    // Code to repeat five times, excluding iteration 2
    Console.WriteLine($"Iteration {i + 1}");
}
```

[Slide 9: Infinite Loops]
- 🔄🔄 The never-ending dance! Infinite loops are loops without a defined exit condition. Be cautious to avoid unintentional infinite loops.

[Slide 10: Benefits of Loops]
- 🌐 The time-saver! Loops enhance code efficiency by automating repetitive tasks, making your programs more concise and maintainable.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've become a choreographer of code with "Repeated Actions" using loops in C#. Today, we explored the for loop, while loop, do-while loop, and common loop practices. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've mastered the art of repetition with loops in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## For Loop

[Opening Slide]
- 🚀 Welcome to another exciting episode of the "C# Fundamentals" course! Today, we're unraveling the magic of the "For Loop" in C#. Brace yourselves for a rhythmic journey through controlled repetition! 🔄🎶🔍

[Slide 1: Introduction to For Loop]
- ➡️ The spotlight is on the for loop! This loop is your go-to maestro when you know exactly how many times you want to repeat a block of code.

[Slide 2: Anatomy of a For Loop]
- 🔢 The conductor's wand! The for loop consists of three main components: initialization, condition, and iteration.
```csharp
for (int i = 0; i < 5; i++)
{
    // Code to repeat five times
    Console.WriteLine($"Iteration {i + 1}");
}
```

[Slide 3: Step-by-Step Breakdown]
- 🚶‍♂️ Let's break it down:
  - Initialization (`int i = 0`): Setting up the loop variable.
  - Condition (`i < 5`): Checking if the condition is true to continue looping.
  - Iteration (`i++`): Incrementing the loop variable after each iteration.

[Slide 4: For Loop Example]
- 🎭 The classic countdown! If you want to create a countdown from 5 to 1:
```csharp
for (int i = 5; i > 0; i--)
{
    Console.WriteLine($"Countdown: {i}");
}
```

[Slide 5: Nested For Loop]
- 🔄🔄 The loop within a loop! For loops can be nested, providing a powerful way to iterate over two-dimensional arrays or perform intricate tasks.
```csharp
for (int i = 1; i <= 3; i++)
{
    for (int j = 1; j <= 3; j++)
    {
        Console.Write($"({i},{j}) ");
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 6: Benefits of For Loop]
- 🌐 The precision dancer! The for loop shines when you have a clear idea of the number of iterations, making your code structured and efficient.

[Slide 7: Breaking Out of For Loop]
- ⛔ The exit strategy! The `break` statement allows you to exit a for loop prematurely, based on a certain condition.

[Slide 8: Skipping Iterations with Continue]
- ⏭️ The dance skipper! The `continue` statement skips the rest of the current iteration and moves to the next one.
```csharp
for (int i = 1; i <= 5; i++)
{
    if (i == 3)
    {
        // Skip the rest of iteration 3
        continue;
    }
    Console.WriteLine($"Iteration {i}");
}
```

[Slide 9: Infinite For Loop]
- 🔄🔄 The never-ending dance! Be cautious with infinite loops. Make sure there's a clear exit condition to avoid unintentional infinite repetition.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've mastered the rhythmic art of the "For Loop" in C#. Today, we explored its structure, saw examples, and even delved into nested loops. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a conductor of code with the "For Loop" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## While Loop

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're stepping into the rhythmic world of the "While Loop" in C#. Get ready for a dance of controlled repetition that adapts to changing conditions! 🔄💃🔍

[Slide 1: Unveiling the While Loop]
- ➡️ The spotlight is on the while loop! Unlike the for loop, the while loop dances to the beat of a condition, repeating as long as that condition holds true.

[Slide 2: Anatomy of a While Loop]
- 🔄 The dance floor! The while loop consists of a single condition that determines whether the loop should continue or break.
```csharp
int counter = 0;
while (counter < 5)
{
    // Code to repeat five times
    Console.WriteLine($"Iteration {counter + 1}");
    counter++;
}
```

[Slide 3: Step-by-Step Breakdown]
- 🚶‍♀️ Let's break it down:
  - Condition (`counter < 5`): The loop continues as long as this condition is true.
  - Code Block: The block of code inside the loop that gets repeated.
  - Iteration (`counter++`): The increment or change in the loop variable to eventually break the loop.

[Slide 4: While Loop Example]
- 🎭 The endless applause! If you want to simulate applause until the audience gets tired:
```csharp
bool audienceApplauding = true;
while (audienceApplauding)
{
    Console.WriteLine("Clap, clap, clap!");
    // Simulating a condition change
    audienceApplauding = /* Get the updated value */;
}
```

[Slide 5: Infinite While Loop]
- 🔄🔄 The never-ending dance! Be cautious with infinite loops. Always ensure there's a mechanism for the loop to eventually break.

[Slide 6: Breaking Out of While Loop]
- ⛔ The exit strategy! The `break` statement allows you to exit a while loop prematurely, based on a certain condition.

[Slide 7: Skipping Iterations with Continue]
- ⏭️ The dance skipper! The `continue` statement skips the rest of the current iteration and moves to the next one.
```csharp
int i = 0;
while (i < 5)
{
    if (i == 2)
    {
        // Skip the rest of iteration 2
        i++;
        continue;
    }
    Console.WriteLine($"Iteration {i + 1}");
    i++;
}
```

[Slide 8: Benefits of While Loop]
- 🌐 The adaptable dancer! While loops are perfect when you don't know the exact number of iterations in advance, allowing your code to adapt to changing conditions.

[Slide 9: When to Use While Loop]
- 🤔 The right move! Use a while loop when the number of iterations isn't predetermined, and the loop should continue until a specific condition is met.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've mastered the rhythmic art of the "While Loop" in C#. Today, we explored its structure, saw examples, and learned about breaking and skipping iterations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a dance choreographer with the "While Loop" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Do-While Loop

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the dynamic beats of the "Do-While Loop" in C#. Get ready for a dance of controlled repetition that guarantees at least one performance! 🔄🕺🔍

[Slide 1: Introducing the Do-While Loop]
- ➡️ The stage is set for the do-while loop! Similar to the while loop, but with a twist—it guarantees at least one execution before checking the loop condition.

[Slide 2: Anatomy of a Do-While Loop]
- 🔄 The dance partner! The do-while loop consists of a code block and a condition, ensuring the block executes at least once.
```csharp
int count = 0;
do
{
    // Code to repeat at least once
    Console.WriteLine($"Iteration {count + 1}");
    count++;
} while (count < 5);
```

[Slide 3: Step-by-Step Breakdown]
- 🚶‍♂️ Let's break it down:
  - Code Block: The block of code inside the loop that gets repeated.
  - Condition (`count < 5`): The loop continues as long as this condition is true.
  - Iteration (`count++`): The increment or change in the loop variable to eventually break the loop.

[Slide 4: Do-While Loop Example]
- 🎭 The encore performance! If you want to play a game with the user until they win:
```csharp
string userResponse;
do
{
    Console.WriteLine("Try again! Do you want to play again? (yes/no)");
    userResponse = Console.ReadLine();
} while (userResponse.ToLower() == "yes");
```

[Slide 5: Breaking Out of Do-While Loop]
- ⛔ The exit strategy! The `break` statement allows you to exit a do-while loop prematurely, based on a certain condition.

[Slide 6: Skipping Iterations with Continue]
- ⏭️ The dance skipper! The `continue` statement skips the rest of the current iteration and moves to the next one.
```csharp
int i = 0;
do
{
    if (i == 2)
    {
        // Skip the rest of iteration 2
        i++;
        continue;
    }
    Console.WriteLine($"Iteration {i + 1}");
    i++;
} while (i < 5);
```

[Slide 7: Infinite Do-While Loop]
- 🔄🔄 The never-ending encore! Be cautious with infinite loops. Always ensure there's a mechanism for the loop to eventually break.

[Slide 8: Benefits of Do-While Loop]
- 🌐 The persistent performer! Do-while loops are perfect when you want to ensure that a block of code is executed at least once, regardless of the initial condition.

[Slide 9: When to Use Do-While Loop]
- 🤔 The encore scenario! Use a do-while loop when you want to guarantee the execution of a block of code at least once, and then continue based on a condition.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've mastered the dynamic moves of the "Do-While Loop" in C#. Today, we explored its structure, saw examples, and learned about breaking and skipping iterations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a dance virtuoso with the "Do-While Loop" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## The "break" Keyword

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into a key player in the world of loops—the "break" keyword. Get ready for a crash course on how to make your loops bow out gracefully! ⚔️🔄🔍

[Slide 1: Unveiling the "break" Keyword]
- ➡️ The stage is set for the "break" keyword! This powerful command allows you to gracefully exit a loop before its natural completion.

[Slide 2: When to Use "break"]
- 🤔 The exit strategy! Use "break" when you want to prematurely terminate a loop based on a specific condition, bringing flexibility and control to your code.

[Slide 3: Anatomy of "break"]
- 🚪 Opening the escape hatch! The "break" keyword is a one-liner that, when encountered, immediately exits the loop.
```csharp
for (int i = 1; i <= 10; i++)
{
    if (i == 5)
    {
        // Exit the loop when i equals 5
        break;
    }
    Console.WriteLine($"Iteration {i}");
}
```

[Slide 4: The "break" Scenario]
- ⛔ The emergency exit! Let's say you're searching for a specific value in an array. Once found, you can break out of the loop.
```csharp
int[] numbers = { 2, 4, 7, 1, 9, 5 };
int target = 7;
for (int i = 0; i < numbers.Length; i++)
{
    if (numbers[i] == target)
    {
        Console.WriteLine($"Target {target} found at index {i}");
        break;
    }
}
```

[Slide 5: Breaking Out of Nested Loops]
- ⛔⛔ Breaking the chains! The "break" keyword is also effective in breaking out of nested loops, providing a quick escape route.
```csharp
for (int i = 1; i <= 5; i++)
{
    for (int j = 1; j <= 5; j++)
    {
        Console.Write($"({i},{j}) ");
        if (j == 3)
        {
            // Exit the inner loop when j equals 3
            break;
        }
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 6: The "break" Considerations]
- ⚖️ Handle with care! While "break" is a handy tool, excessive use might make your code less readable. Use it judiciously to maintain code clarity.

[Slide 7: Combining "break" with Conditional Statements]
- 🎭 The dynamic duo! Combine "break" with conditional statements for nuanced control over loop termination.
```csharp
int[] numbers = { 3, 7, 1, 8, 4, 2 };
for (int i = 0; i < numbers.Length; i++)
{
    if (numbers[i] % 2 == 0)
    {
        Console.WriteLine($"First even number found: {numbers[i]} at index {i}");
        break;
    }
}
```

[Slide 8: Benefits of "break"]
- 🌐 The emergency exit door! "break" provides a quick and efficient way to exit loops, adding a layer of dynamism to your code.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've become the maestro of loop exits with the "break" keyword in C#. Today, we explored its use, scenarios, and considerations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've mastered the art of loop control with the "break" keyword in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## The "continue" Keyword

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're exploring another powerful tool in the world of loops—the "continue" keyword. Get ready to skip to the next beat and keep your loops grooving! ⏭️🔄🔍

[Slide 1: Unveiling the "continue" Keyword]
- ➡️ The stage is set for the "continue" keyword! This nifty command allows you to skip the rest of the current iteration and move directly to the next one.

[Slide 2: When to Use "continue"]
- 🤔 The rhythm keeper! Use "continue" when you want to skip specific iterations based on a condition, keeping your loop in sync with your coding melody.

[Slide 3: Anatomy of "continue"]
- ⏩ Skipping a beat! The "continue" keyword, when encountered, immediately jumps to the next iteration of the loop, skipping the rest of the current iteration.
```csharp
for (int i = 1; i <= 5; i++)
{
    if (i % 2 == 0)
    {
        // Skip the rest of the iteration for even numbers
        continue;
    }
    Console.WriteLine($"Iteration {i}");
}
```

[Slide 4: The "continue" Scenario]
- 🎵 The silent beats! Let's say you want to print all odd numbers from an array but skip the even ones:
```csharp
int[] numbers = { 2, 5, 8, 3, 6, 9 };
for (int i = 0; i < numbers.Length; i++)
{
    if (numbers[i] % 2 == 0)
    {
        // Skip the rest of the iteration for even numbers
        continue;
    }
    Console.WriteLine($"Odd number found: {numbers[i]}");
}
```

[Slide 5: Skipping in Nested Loops]
- ⏭️⏭️ Skipping between layers! The "continue" keyword is equally effective in nested loops, allowing you to skip specific iterations in both the inner and outer loops.
```csharp
for (int i = 1; i <= 3; i++)
{
    for (int j = 1; j <= 3; j++)
    {
        if (j == 2)
        {
            // Skip the rest of the inner loop for j equals 2
            continue;
        }
        Console.Write($"({i},{j}) ");
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 6: The "continue" Considerations]
- ⚖️ Harmonize wisely! While "continue" adds flexibility, be mindful of its use. Excessive skipping may affect the readability of your code.

[Slide 7: Combining "continue" with Conditional Statements]
- 🎭 The dynamic duo! Combine "continue" with conditional statements for nuanced control over which iterations to skip.
```csharp
string[] fruits = { "Apple", "Banana", "Grapes", "Kiwi", "Orange" };
for (int i = 0; i < fruits.Length; i++)
{
    if (fruits[i].Length > 5)
    {
        // Skip the rest of the iteration for longer fruit names
        continue;
    }
    Console.WriteLine($"Short fruit name found: {fruits[i]}");
}
```

[Slide 8: Benefits of "continue"]
- 🎶 Skipping beats with grace! "continue" provides a seamless way to skip specific iterations, adding finesse to your loop compositions.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've become the choreographer of loop skips with the "continue" keyword in C#. Today, we explored its use, scenarios, and considerations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've mastered the art of skipping beats with the "continue" keyword in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep coding to your rhythm! 🎉

## Nested Loops

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the fascinating world of nested loops. Get ready to unravel the intricacies of loops within loops! 🔄🔄🕵️‍♂️

[Slide 1: Unveiling Nested Loops]
- ➡️ The stage is set for nested loops! In C#, we have the flexibility to place loops inside one another, creating a dynamic and powerful rhythm of repetition.

[Slide 2: Why Nested Loops?]
- 🤔 The symphony of complexity! Nested loops are instrumental when dealing with multidimensional data structures, matrices, or patterns that require layered iteration.

[Slide 3: Anatomy of Nested Loops]
- 🔄🔄 The loop symphony! Nesting involves placing one loop inside the body of another, creating a harmony of repetitive actions.
```csharp
for (int i = 1; i <= 3; i++)
{
    for (int j = 1; j <= 3; j++)
    {
        Console.Write($"({i},{j}) ");
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 4: Step-by-Step Breakdown]
- 🚶‍♂️ Let's break it down:
  - Outer Loop (`for (int i = 1; i <= 3; i++)`): Controls the repetition of the entire nested structure.
  - Inner Loop (`for (int j = 1; j <= 3; j++)`): Executes inside the body of the outer loop, creating a repetitive pattern.

[Slide 5: Nested Loop Example - Matrix]
- 🎨 The matrix masterpiece! Nested loops are ideal for working with matrices or 2D arrays.
```csharp
int[,] matrix = new int[3, 3];
for (int i = 0; i < 3; i++)
{
    for (int j = 0; j < 3; j++)
    {
        matrix[i, j] = i + j;
        Console.Write($"{matrix[i, j]} ");
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 6: Nested Loop Example - Pattern]
- 🌌 The pattern weaver! Nested loops can create intricate patterns with their synchronized repetitions.
```csharp
for (int i = 1; i <= 5; i++)
{
    for (int j = 1; j <= i; j++)
    {
        Console.Write($"{j} ");
    }
    Console.WriteLine(); // Move to the next line after inner loop completes
}
```

[Slide 7: Nested Loop Considerations]
- ⚖️ Harmony and balance! While nested loops are powerful, be mindful of their potential complexity. Ensure clarity in your code to maintain readability.

[Slide 8: Benefits of Nested Loops]
- 🎭 The ensemble performance! Nested loops offer a versatile way to handle intricate data structures and create complex patterns in your code.

[Slide 9: When to Use Nested Loops]
- 🤔 The layered scenario! Use nested loops when dealing with multidimensional data, matrices, or scenarios that require a structured repetition within another repetition.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've mastered the symphony of nested loops in C#. Today, we explored their structure, saw examples with matrices and patterns, and discussed considerations. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become the conductor of nested loops in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep orchestrating with nested loops! 🎉

## Drawing Patterns

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unleashing our creative side by exploring how to draw patterns using C#. Get ready to turn your code into a canvas! 🎨🔄✨

[Slide 1: The Art of Drawing Patterns]
- ➡️ Let's dive into the artistry of drawing patterns in C#! Patterns add a touch of creativity to your code and are often created using nested loops.

[Slide 2: Importance of Patterns]
- 🤔 Why draw patterns in code? Patterns are not just visually appealing; they also enhance your understanding of loops, logic, and control flow.

[Slide 3: Basic Patterns - Pyramid]
- 🏰 The pyramid masterpiece! Let's start with a classic pattern—a pyramid.
```csharp
int rows = 5;
for (int i = 1; i <= rows; i++)
{
    for (int j = 1; j <= i; j++)
    {
        Console.Write("* ");
    }
    Console.WriteLine();
}
```

[Slide 4: Basic Patterns - Reverse Pyramid]
- 🔄 The inverse creation! Now, let's flip the pyramid upside down.
```csharp
int rows = 5;
for (int i = rows; i >= 1; i--)
{
    for (int j = 1; j <= i; j++)
    {
        Console.Write("* ");
    }
    Console.WriteLine();
}
```

[Slide 5: Advanced Patterns - Diamond]
- 💎 The diamond challenge! Creating a diamond pattern requires a bit more complexity.
```csharp
int rows = 5;
int spaces = rows - 1;
for (int i = 1; i <= rows; i++)
{
    for (int j = 1; j <= spaces; j++)
    {
        Console.Write(" ");
    }
    spaces--;

    for (int j = 1; j <= 2 * i - 1; j++)
    {
        Console.Write("*");
    }
    Console.WriteLine();
}
```

[Slide 6: Advanced Patterns - Hollow Square]
- 🏰✨ The hollow square magic! Constructing a hollow square pattern requires a combination of loops.
```csharp
int rows = 5;
for (int i = 1; i <= rows; i++)
{
    for (int j = 1; j <= rows; j++)
    {
        if (i == 1 || i == rows || j == 1 || j == rows)
        {
            Console.Write("* ");
        }
        else
        {
            Console.Write("  ");
        }
    }
    Console.WriteLine();
}
```

[Slide 7: Experimenting with Your Own Patterns]
- 🚀 Time to become an artist! Once you grasp the basics, experiment with your own patterns. Mix and match loops to create unique designs!

[Slide 8: Benefits of Drawing Patterns]
- 🌈 Beyond aesthetics! Drawing patterns in code enhances your problem-solving skills, boosts creativity, and solidifies your understanding of loops and conditions.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've ventured into the world of drawing patterns in C#. Today, we explored basic and advanced patterns, understanding the magic behind the loops. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You're now a pattern artist in C#. Join us next time for more insights and hands-on coding adventures. Until then, keep creating with patterns! 🎉✨