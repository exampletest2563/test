# 🔀 Control Flow - Conditional Statements

## 💡 Conditional Statements

In any programming language, the code needs to make decisions and carry out actions depending on different inputs.

`Pseudocode`

```csharp
if (condition)
{
	// Code to be executed if condition is true
}
else
{
	// Code to be executed if condition is false
}
```

In this example the word `condition` could be replaced with one of the following:
- a literal of type `bool`;
- a variable of type `bool`;
- any expression that could be evaluated to a value of type `bool`.

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the world of "Conditional Statements" in C#. Get ready to make your programs smart and responsive by navigating the pathways of decision-making! 🛣️🤔

[Slide 1: The Power of Decision-Making]
- ➡️ Conditional statements are the architects of intelligent programs. They allow your code to make decisions based on specific conditions, creating dynamic and responsive applications.

[Slide 2: if Statements]
- 🎭 Let's start with the classic drama of `if` statements. This fundamental construct allows your program to execute a block of code only if a specified condition is true.

[Slide 3: Example - if Statement]
- 🚦 Light the way! If you want to check if a number is positive, you can use:
```csharp
int number = 42;
if (number > 0)
{
    Console.WriteLine("The number is positive!");
}
```

[Slide 4: if-else Statements]
- ↔️ Enter the dualistic world of `if-else` statements. If the condition is true, one block of code is executed; otherwise, another block takes the stage.

[Slide 5: Example - if-else Statement]
- 🚪 Choose your path! If you want to check if a number is even or odd, you can use:
```csharp
int number = 42;
if (number % 2 == 0)
{
    Console.WriteLine("The number is even!");
}
else
{
    Console.WriteLine("The number is odd!");
}
```

[Slide 6: if-else if-else Statements]
- 🎭 The grand performance of `if-else if-else` statements! This allows your program to evaluate multiple conditions in sequence, executing the block associated with the first true condition.

[Slide 7: Example - if-else if-else Statement]
- 🌐 A journey of conditions! If you want to classify a student's grade, you can use:
```csharp
int score = 75;
if (score >= 90)
{
    Console.WriteLine("A");
}
else if (score >= 80)
{
    Console.WriteLine("B");
}
else if (score >= 70)
{
    Console.WriteLine("C");
}
else
{
    Console.WriteLine("Fail");
}
```

[Slide 8: switch Statements]
- 🚦 The versatile `switch` statement takes center stage! It evaluates a variable against multiple possible values and executes the block associated with the first match.

[Slide 9: Example - switch Statement]
- 🌟 The switch performance! If you want to handle different day names, you can use:
```csharp
string day = "Monday";
switch (day)
{
    case "Monday":
        Console.WriteLine("It's the start of the week!");
        break;
    case "Friday":
        Console.WriteLine("Hello, weekend!");
        break;
    default:
        Console.WriteLine("It's a regular day.");
        break;
}
```

[Slide 10: Conditional Ternary Operator]
- 🔄 The compact `ternary operator` is your secret agent for concise decision-making. It's a shorthand way of expressing simple `if-else` statements.

[Slide 11: Example - Ternary Operator]
- 🎯 The swift ternary! If you want to determine if a number is positive or negative, you can use:
```csharp
int number = 42;
string result = (number > 0) ? "Positive" : "Negative";
Console.WriteLine($"The number is {result}!");
```

[Slide 12: Benefits of Conditional Statements]
- 🌈 Conditional statements empower your programs to adapt and respond dynamically. Whether it's making decisions, handling multiple scenarios, or expressing concise choices, mastering conditionals is a key skill in programming.

[Slide 13: Recap and Next Steps]
- 🎓 Bravo! You've mastered the art of "Conditional Statements" in C#. Today, we explored `if`, `if-else`, `if-else if-else`, `switch`, and the ternary operator. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've unlocked the doors of decision-making in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Boolean Expressions

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're delving into the realm of "Boolean Expressions" in C#. Get ready to unravel the logic behind decision-making and condition evaluation! 🧠🔍

[Slide 1: The Logic Behind Boolean Expressions]
- ➡️ Boolean expressions are the detectives of your code, determining whether a condition is true or false. They form the foundation of decision-making and control flow in your programs.

[Slide 2: True and False Values]
- ✔️✖️ In the world of boolean expressions, everything boils down to two values: `true` and `false`. These values dictate the flow of your code based on the conditions you set.

[Slide 3: Comparison Operators]
- 🤔 Comparison operators are the tools of the trade! They allow you to compare values and create boolean expressions. From equality to inequality, these operators help you express conditions.

[Slide 4: Example - Comparison Operators]
- 🧐 The comparison game! If you want to check if a number is greater than or equal to 10, you can use:
```csharp
int number = 15;
bool isGreaterThanTen = (number >= 10);
Console.WriteLine($"Is the number greater than or equal to 10? {isGreaterThanTen}");
```

[Slide 5: Logical Operators]
- 🌐 Logical operators connect the dots! They allow you to combine multiple boolean expressions, creating complex conditions that drive decision-making in your programs.

[Slide 6: Example - Logical Operators]
- 🔗 The logical puzzle! If you want to check if a number is between 10 and 20, you can use the logical AND (`&&`) operator:
```csharp
int number = 15;
bool isBetweenTenAndTwenty = (number >= 10) && (number <= 20);
Console.WriteLine($"Is the number between 10 and 20? {isBetweenTenAndTwenty}");
```

[Slide 7: Boolean Variables]
- 📦 Boolean variables are your trusty allies! They store the result of boolean expressions, allowing you to refer to the outcome later in your code.

[Slide 8: Example - Boolean Variables]
- 🎭 The boolean performer! If you want to check if a user is logged in, you can use a boolean variable:
```csharp
bool isLoggedIn = /* Some authentication logic */;
if (isLoggedIn)
{
    Console.WriteLine("Welcome, user!");
}
else
{
    Console.WriteLine("Please log in to access the content.");
}
```

[Slide 9: Negation Operator]
- 🔄 The negation operator (`!`) is the flipper! It changes a `true` value to `false` and vice versa. It's like turning on the light in a dark room.

[Slide 10: Example - Negation Operator]
- 🌓 Flipping the switch! If you want to check if a user is not an admin, you can use:
```csharp
bool isAdmin = /* Some admin check */;
if (!isAdmin)
{
    Console.WriteLine("You don't have admin privileges.");
}
```

[Slide 11: Benefits of Boolean Expressions]
- 🌈 Boolean expressions are the architects of decision-making in your programs. They allow you to create conditions, make choices, and control the flow of your code based on logical evaluations.

[Slide 12: Recap and Next Steps]
- 🎓 Bravo! You've mastered the art of "Boolean Expressions" in C#. Today, we explored comparison operators, logical operators, boolean variables, and the negation operator. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a logic maestro with "Boolean Expressions" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## IF Statement

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're embarking on a journey into the world of "IF Statements" in C#. Get ready to uncover the power of decision-making in your code! 🚦🤔

[Slide 1: The Essence of IF Statements]
- ➡️ IF statements are the gatekeepers of your code, allowing it to make decisions based on specified conditions. These decision points add a layer of intelligence, making your programs dynamic and responsive.

[Slide 2: Anatomy of an IF Statement]
- 🎭 Let's break down the theatrical performance of an IF statement. It consists of the keyword `if`, a condition enclosed in parentheses, and a block of code to execute if the condition is true.

[Slide 3: Example - Basic IF Statement]
- 🚦 The classic spotlight! If you want to check if a number is positive, you can use:
```csharp
int number = 42;
if (number > 0)
{
    Console.WriteLine("The number is positive!");
}
```

[Slide 4: Using Comparison Operators in IF Statements]
- 🕵️‍♂️ Comparison operators are the detectives in your conditions. From equality to inequality, they help you express the logic behind your decisions.

[Slide 5: Example - Using Comparison Operators]
- 🧐 Sherlock, the code detective! If you want to check if a user's age is 18 or older, you can use:
```csharp
int userAge = /* Get user's age */;
if (userAge >= 18)
{
    Console.WriteLine("You're eligible for access!");
}
```

[Slide 6: Nesting IF Statements]
- 🏰 The castle of decisions! You can nest IF statements within each other to create more complex conditions and handle various scenarios.

[Slide 7: Example - Nesting IF Statements]
- 🎭 The nested drama! If you want to check both age and whether the user has an account, you can use:
```csharp
int userAge = /* Get user's age */;
bool hasAccount = /* Check if user has an account */;
if (userAge >= 18)
{
    if (hasAccount)
    {
        Console.WriteLine("Welcome, valued user!");
    }
    else
    {
        Console.WriteLine("You need to create an account.");
    }
}
else
{
    Console.WriteLine("Access restricted to users 18 and older.");
}
```

[Slide 8: Benefits of IF Statements]
- 🌈 IF statements empower your code to adapt and respond dynamically. They allow your programs to choose different paths based on conditions, enhancing the overall intelligence of your applications.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've explored the magic of "IF Statements" in C#. Today, we dissected the anatomy of IF statements, used comparison operators, and even ventured into nested IF statements. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've unlocked the gates of decision-making with "IF Statements" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## IF-ELSE Statement

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the expressive world of "IF-ELSE Statements" in C#. Get ready to unfold the story of decision-making with dual paths in your code! 🚦🤔

[Slide 1: The Dynamic Duo - IF-ELSE Statements]
- ➡️ IF-ELSE statements are like having a superhero duo in your code. They enable your programs to take one path if a condition is true and another if it's false, adding versatility to your decision-making.

[Slide 2: Anatomy of an IF-ELSE Statement]
- 🎭 The IF-ELSE statement is a script with a twist. It features the familiar `if` keyword, a condition in parentheses, a block of code for the true scenario, followed by the `else` keyword and another block of code for the false scenario.

[Slide 3: Example - Basic IF-ELSE Statement]
- 🚦 The dual performance! If you want to check if a number is even or odd, you can use:
```csharp
int number = 42;
if (number % 2 == 0)
{
    Console.WriteLine("The number is even!");
}
else
{
    Console.WriteLine("The number is odd!");
}
```

[Slide 4: The Power of Alternatives]
- ↔️ Alternatives at your fingertips! IF-ELSE statements allow your code to gracefully handle different scenarios, making decisions based on the conditions you set.

[Slide 5: Example - IF-ELSE for Grade Classification]
- 🎓 A grading masterpiece! If you want to classify a student's grade, you can use:
```csharp
int score = 75;
if (score >= 90)
{
    Console.WriteLine("A");
}
else if (score >= 80)
{
    Console.WriteLine("B");
}
else if (score >= 70)
{
    Console.WriteLine("C");
}
else
{
    Console.WriteLine("Fail");
}
```

[Slide 6: Nesting IF-ELSE Statements]
- 🏰 The castle expands! You can nest IF-ELSE statements within each other, creating intricate decision trees for more complex scenarios.

[Slide 7: Example - Nested IF-ELSE for Age and Account Check]
- 🎭 The nested drama! If you want to check both age and whether the user has an account, you can use:
```csharp
int userAge = /* Get user's age */;
bool hasAccount = /* Check if user has an account */;
if (userAge >= 18)
{
    if (hasAccount)
    {
        Console.WriteLine("Welcome, valued user!");
    }
    else
    {
        Console.WriteLine("You need to create an account.");
    }
}
else
{
    Console.WriteLine("Access restricted to users 18 and older.");
}
```

[Slide 8: Benefits of IF-ELSE Statements]
- 🌈 IF-ELSE statements bring flexibility and adaptability to your code. They let your programs make choices and navigate different paths, ensuring a dynamic and responsive user experience.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've explored the dynamic world of "IF-ELSE Statements" in C#. Today, we dissected the anatomy, embraced alternatives, and even ventured into nested scenarios. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've mastered the dual paths of decision-making with "IF-ELSE Statements" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Variables Scope & Visibility

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the fascinating realm of "Variables Scope & Visibility" in C#. Get ready to explore where your variables live and who gets to see them! 🔍🏠

[Slide 1: Understanding Scope]
- 🧭 Scope defines the region of your code where a variable is accessible. It's like the neighborhood where a variable resides, and its rules determine who can interact with it.

[Slide 2: Local Variables - The Neighborhood Residents]
- 🏡 Local variables have a local address! They live within a specific block of code, such as a method or a loop. Once you step out of that block, they vanish.

[Slide 3: Example - Local Variables]
- 🚪 Local living! If you declare a variable inside a method, it's local to that method:
```csharp
void MyMethod()
{
    int localVar = 42; // Local variable
    Console.WriteLine(localVar);
    // localVar is accessible here
}
// localVar is not accessible here
```

[Slide 4: Block Scope]
- 🧱 Blocks create neighborhoods! Variables declared within a block, like in an `if` statement or a loop, have limited visibility within that block.

[Slide 5: Example - Block Scope]
- 🏰 Block residency! If you declare a variable inside an `if` statement, it's local to that block:
```csharp
if (condition)
{
    int blockVar = 10; // Block-scoped variable
    Console.WriteLine(blockVar);
    // blockVar is accessible here
}
// blockVar is not accessible here
```

[Slide 6: Method Scope]
- 🚀 Method is the town! Variables declared at the beginning of a method have the entire method as their scope. They're like the town square where everyone can see them.

[Slide 7: Example - Method Scope]
- 🌆 Method visibility! Variables declared at the beginning of a method are accessible throughout the method:
```csharp
void MyMethod()
{
    int methodVar = 5; // Method-scoped variable
    Console.WriteLine(methodVar);
    // methodVar is accessible here
}
// methodVar is not accessible here
```

[Slide 8: Class Scope]
- 🌍 Class is the city! Variables declared at the class level are visible to all methods within that class. They have the broadest visibility.

[Slide 9: Example - Class Scope]
- 🌃 Class visibility! Variables declared at the class level are accessible throughout the class:
```csharp
class MyClass
{
    int classVar = 20; // Class-scoped variable
    void Method1()
    {
        Console.WriteLine(classVar);
        // classVar is accessible here
    }
    void Method2()
    {
        Console.WriteLine(classVar);
        // classVar is accessible here
    }
}
```

[Slide 10: Visibility Modifiers]
- 🔒 Open or closed gates! You can control the visibility of variables using visibility modifiers like `public`, `private`, `protected`, and `internal`.

[Slide 11: Example - Visibility Modifiers]
- 🚧 Gatekeeper choices! If you want to restrict access to a variable, you can use a private modifier:
```csharp
class MyClass
{
    private int privateVar = 30; // Private variable
    // Other members of the class can access privateVar
}
// Outside the class, privateVar is not accessible
```

[Slide 12: Benefits of Understanding Scope & Visibility]
- 🌈 Mastering scope and visibility empowers you to organize your code effectively, control access to variables, and build robust and modular programs.

[Slide 13: Recap and Next Steps]
- 🎓 Bravo! You've navigated the neighborhoods of "Variables Scope & Visibility" in C#. Today, we explored local, block, method, and class scopes, and learned about visibility modifiers. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a master urban planner of variables with "Variables Scope & Visibility" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Multiple Conditions

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unraveling the mystery of "Multiple Conditions" in C#. Get ready to combine logic like a pro and enhance your decision-making skills! 🤹‍♂️🔍

[Slide 1: The Complexity of Decision-Making]
- ➡️ Sometimes, decisions are not black or white. They involve multiple conditions, and that's where the magic of "Multiple Conditions" comes into play.

[Slide 2: Logical AND Operator - &&]
- 🔗 The logical conjunction! The AND operator (`&&`) allows you to create conditions that require all specified criteria to be true.

[Slide 3: Example - Logical AND Operator]
- 🌐 The teamwork scenario! If you want to check if a person is both an adult and has a driver's license, you can use:
```csharp
int age = 25;
bool hasLicense = true;
if (age >= 18 && hasLicense)
{
    Console.WriteLine("You can drive!");
}
```

[Slide 4: Logical OR Operator - ||]
- 🌈 The inclusive choice! The OR operator (`||`) lets you create conditions where at least one of the specified criteria needs to be true.

[Slide 5: Example - Logical OR Operator]
- 🎭 The weekend plan! If you want to check if a day is either Saturday or Sunday, you can use:
```csharp
string day = "Sunday";
if (day == "Saturday" || day == "Sunday")
{
    Console.WriteLine("It's the weekend!");
}
```

[Slide 6: Logical NOT Operator - !]
- 🔄 The reversal trick! The NOT operator (`!`) negates a condition, flipping it from true to false or vice versa.

[Slide 7: Example - Logical NOT Operator]
- 🚫 The exclusive club! If you want to check if a person is not a VIP, you can use:
```csharp
bool isVIP = /* Check if person is a VIP */;
if (!isVIP)
{
    Console.WriteLine("You're not a VIP. Welcome!");
}
```

[Slide 8: Combining Multiple Conditions]
- 🎨 The masterpiece of logic! You can combine multiple conditions using logical AND, OR, and NOT operators to create intricate decision trees.

[Slide 9: Example - Combining Conditions]
- 🌲 The forest of decisions! If you want to check if a person is eligible for a discount based on age and membership, you can use:
```csharp
int age = 22;
bool isMember = true;
if ((age >= 18 && age <= 30) || isMember)
{
    Console.WriteLine("You qualify for a discount!");
}
```

[Slide 10: Benefits of Multiple Conditions]
- 🌐 Mastering multiple conditions empowers you to express complex decision-making in your code. It's the key to handling diverse scenarios and creating intelligent programs.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've conquered the art of "Multiple Conditions" in C#. Today, we explored logical AND, OR, and NOT operators, and combined them to make intricate decisions. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've unlocked the secrets of complex decision-making with "Multiple Conditions" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Nested Conditional Statements

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're delving into the fascinating world of "Nested Conditional Statements" in C#. Get ready to explore the layers of decision-making and create intricate logic structures! 🏰🔍

[Slide 1: The Depths of Decision-Making]
- ➡️ Sometimes, decisions aren't linear—they're nested. Nested conditional statements allow you to create decision trees with multiple layers, unlocking a new dimension of logic.

[Slide 2: What are Nested Conditional Statements?]
- 🔄 Layers of decisions! Nested conditional statements involve placing one decision inside another. It's like opening a door to another decision room based on the outcome of the first.

[Slide 3: Example - Simple Nesting]
- 🚪 The nested door! If you want to check both age and whether a person has a membership, you can use simple nesting:
```csharp
int age = 25;
bool hasMembership = true;

if (age >= 18)
{
    if (hasMembership)
    {
        Console.WriteLine("Welcome! You have access.");
    }
    else
    {
        Console.WriteLine("You need to purchase a membership.");
    }
}
else
{
    Console.WriteLine("Access restricted to users 18 and older.");
}
```

[Slide 4: Avoiding Complex Nesting - ELSE IF]
- 🔍 The else if option! Instead of deep nesting, you can use else if to create a more readable structure, avoiding the "pyramid of doom."

[Slide 5: Example - Using ELSE IF]
- 🏰 The alternative castle! The same scenario using else if:
```csharp
int age = 25;
bool hasMembership = true;

if (age >= 18 && hasMembership)
{
    Console.WriteLine("Welcome! You have access.");
}
else if (age >= 18 && !hasMembership)
{
    Console.WriteLine("You need to purchase a membership.");
}
else
{
    Console.WriteLine("Access restricted to users 18 and older.");
}
```

[Slide 6: Benefits of Nested Conditional Statements]
- 🌐 Nesting provides a structured way to handle complex scenarios. It helps maintain code readability and allows you to express intricate logic in a more organized fashion.

[Slide 7: Nested Loops - A Glimpse]
- 🔄 Nested world of loops! Nested conditional statements have a sibling in nested loops, where you can repeat decisions in a structured manner.

[Slide 8: Example - Nested Loop (Quick Teaser)]
- 🔄 Looping through layers! A quick teaser of a nested loop scenario:
```csharp
for (int i = 0; i < 5; i++)
{
    for (int j = 0; j < 3; j++)
    {
        Console.Write($"{i}-{j} ");
    }
    Console.WriteLine();
}
```

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've navigated the layers of "Nested Conditional Statements" in C#. Today, we explored the concept, saw examples of simple and structured nesting, and glimpsed into the world of nested loops. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've mastered the art of layered decision-making with "Nested Conditional Statements" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Building Complex Boolean Expressions

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're embarking on the exciting journey of "Building Complex Boolean Expressions" in C#. Get ready to craft intricate logic and unlock the power of boolean expressions! 🛠️🔍

[Slide 1: The Art of Crafting Complexity]
- ➡️ Building complex boolean expressions is like crafting a puzzle where each piece adds meaning to the whole. It's about creating sophisticated conditions for your code to navigate.

[Slide 2: The Building Blocks - Logical Operators]
- 🔧 The tools of the trade! Logical operators (AND, OR, NOT) are the building blocks for constructing complex boolean expressions.

[Slide 3: Example - Combining Conditions with AND (&&)]
- 🌐 The teamwork puzzle! If you want to check if a person is an adult, has a membership, and the account is active, you can use the AND operator:
```csharp
int age = 25;
bool hasMembership = true;
bool isAccountActive = true;

if (age >= 18 && hasMembership && isAccountActive)
{
    Console.WriteLine("Welcome! You have full access.");
}
```

[Slide 4: Example - Combining Conditions with OR (||)]
- 🌈 The inclusive puzzle! If you want to check if a person is either a premium or a VIP member, you can use the OR operator:
```csharp
bool isPremiumMember = /* Check if person is a premium member */;
bool isVIPMember = /* Check if person is a VIP member */;

if (isPremiumMember || isVIPMember)
{
    Console.WriteLine("You have special privileges!");
}
```

[Slide 5: Example - Combining Conditions with NOT (!)]
- 🔄 The reversal puzzle! If you want to check if a person is not a guest, you can use the NOT operator:
```csharp
bool isGuest = /* Check if person is a guest */;

if (!isGuest)
{
    Console.WriteLine("Welcome! You're not a guest.");
}
```

[Slide 6: Complex Expressions - Mixing AND, OR, and NOT]
- 🌐 The grand puzzle! You can combine multiple conditions using a mix of AND, OR, and NOT to create complex boolean expressions.

[Slide 7: Example - Complex Boolean Expression]
- 🎭 The intricate masterpiece! If you want to check if a person is either a premium or VIP member, aged between 25 and 40, and the account is not blocked, you can use:
```csharp
bool isPremiumMember = /* Check if person is a premium member */;
bool isVIPMember = /* Check if person is a VIP member */;
int age = /* Get person's age */;
bool isAccountBlocked = /* Check if account is blocked */;

if ((isPremiumMember || isVIPMember) && age >= 25 && age <= 40 && !isAccountBlocked)
{
    Console.WriteLine("Welcome! You meet the criteria.");
}
```

[Slide 8: Benefits of Complex Boolean Expressions]
- 🌐 Mastering complex boolean expressions allows you to create nuanced conditions, making your code more adaptable and responsive to diverse scenarios.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've conquered the art of "Building Complex Boolean Expressions" in C#. Today, we explored combining conditions using AND, OR, and NOT operators to create intricate logic. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a master architect of logic with "Building Complex Boolean Expressions" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Switch Statement

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the powerful world of the "Switch Statement" in C#. Get ready to simplify your decision-making with this versatile tool! 🎛️🔍

[Slide 1: The Need for a Switch Statement]
- ➡️ Sometimes, your code needs to make decisions based on the value of a variable. The switch statement provides a clean and efficient solution for handling multiple possible values.

[Slide 2: The Basics of Switch]
- 🔄 The decision maker! The switch statement evaluates an expression and executes the code associated with the matching case.

[Slide 3: Syntax of Switch Statement]
- 📜 The script! The basic syntax of a switch statement:
```csharp
switch (expression)
{
    case value1:
        // Code to execute if expression matches value1
        break;
    case value2:
        // Code to execute if expression matches value2
        break;
    // More cases as needed
    default:
        // Code to execute if no case matches
        break;
}
```

[Slide 4: Example - Simple Switch]
- 🚦 The traffic light scenario! If you want to take actions based on the color of a traffic light:
```csharp
string lightColor = "red";

switch (lightColor)
{
    case "red":
        Console.WriteLine("Stop!");
        break;
    case "yellow":
        Console.WriteLine("Slow down!");
        break;
    case "green":
        Console.WriteLine("Go!");
        break;
    default:
        Console.WriteLine("Invalid color");
        break;
}
```

[Slide 5: Fall-Through Behavior]
- 🍂 The fall-through magic! Unlike some other languages, C# switch statements don't automatically fall through to subsequent cases. Each case must end with a break or other exit statement.

[Slide 6: Multiple Cases for a Single Execution]
- 🎭 The multitasking switch! You can group multiple cases to execute the same block of code:
```csharp
int dayOfWeek = 3;

switch (dayOfWeek)
{
    case 1:
    case 2:
    case 3:
    case 4:
    case 5:
        Console.WriteLine("It's a weekday.");
        break;
    case 6:
    case 7:
        Console.WriteLine("It's the weekend!");
        break;
    default:
        Console.WriteLine("Invalid day");
        break;
}
```

[Slide 7: Switch Expression (C# 8.0 and Later)]
- 🚀 The evolution! Starting from C# 8.0, you can use switch expressions, a more concise and expressive form of the switch statement.

[Slide 8: Example - Switch Expression]
- 🎭 The modern switch! The same weekday-weekend scenario using a switch expression:
```csharp
int dayOfWeek = 3;

string dayType = dayOfWeek switch
{
    >= 1 and <= 5 => "weekday",
    >= 6 and <= 7 => "weekend",
    _ => "invalid day"
};

Console.WriteLine($"It's a {dayType}.");
```

[Slide 9: Benefits of Using Switch]
- 🌐 The organized decision-maker! Switch statements enhance code readability, especially when dealing with multiple possible values. They make your code more structured and easier to maintain.

[Slide 10: Recap and Next Steps]
- 🎓 Bravo! You've mastered the "Switch Statement" in C#. Today, we explored the basic syntax, fall-through behavior, and even glimpsed into the world of switch expressions. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become a decision-making maestro with the "Switch Statement" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Conditional Operator

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're unlocking the magic of the "Conditional Operator" in C#. Get ready to make concise decisions and streamline your code with this powerful operator! 🌟🔍

[Slide 1: The Power of Ternary Operator]
- ➡️ The conditional operator, often called the ternary operator, provides a concise way to make decisions within a single line of code.

[Slide 2: Syntax of Conditional Operator]
- 📜 The script! The basic syntax of the conditional operator:
```csharp
result = (condition) ? trueExpression : falseExpression;
```

[Slide 3: Example - Basic Conditional Operator]
- 🎭 The day or night scenario! If you want to determine if it's daytime or nighttime based on a boolean variable:
```csharp
bool isDaytime = /* Get the value */;
string timeOfDay = (isDaytime) ? "Day" : "Night";
Console.WriteLine($"It's {timeOfDay}time.");
```

[Slide 4: Nesting Conditional Operators]
- 🏰 The nested decision! You can nest conditional operators for more complex scenarios, but be cautious not to sacrifice readability.
```csharp
int temperature = /* Get the value */;
string weatherType = (temperature > 25) ? "Hot" : (temperature < 10) ? "Cold" : "Moderate";
Console.WriteLine($"The weather is {weatherType}.");
```

[Slide 5: Benefits of Conditional Operator]
- 🌐 The concise decision-maker! The conditional operator is perfect for simple decisions, making your code more compact and often improving readability.

[Slide 6: When to Use Conditional Operator]
- 🤔 The right tool for the job! Use the conditional operator when making simple decisions with clear true/false outcomes. For more complex scenarios, consider using other decision-making constructs like if-else statements or switch.

[Slide 7: Limitations of Conditional Operator]
- 🚫 The simplicity trade-off! While the conditional operator is concise, avoid using it excessively or for complex logic. In such cases, traditional control flow structures might be more readable.

[Slide 8: Conditional Operator vs. If-Else]
- ↔️ The comparison! The conditional operator is a great fit for short, simple decisions. If-else statements, on the other hand, offer more flexibility and readability for complex scenarios.

[Slide 9: Recap and Next Steps]
- 🎓 Bravo! You've mastered the "Conditional Operator" in C#. Today, we explored its syntax, saw examples of basic and nested usage, and discussed when to use it. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've added a powerful tool to your coding toolkit with the "Conditional Operator" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉