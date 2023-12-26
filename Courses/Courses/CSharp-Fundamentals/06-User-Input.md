# ✍️ User Input

## I/O Operations

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're diving into the essential topic of "I/O Operations" in C#. Get ready to explore the world of input and output, where your programs communicate with the outside world! 📥📤

[Slide 1: Introduction to I/O Operations]
- ➡️ Input/Output (I/O) operations are the lifeblood of many programs, allowing them to interact with users, read from files, and write to external sources. It's like the conversation between your program and the world.

[Slide 2: Console I/O]
- 🖥️ Let's start with the basics! Console I/O involves interacting with the console window. You can use `Console.WriteLine` to display output and `Console.ReadLine` to get input from the user. It's the simplest way to communicate with your program.

[Slide 3: Example - Console I/O]
- 🚀 Dive into the console world! If you want to greet the user, you can use `Console.WriteLine("Hello, user!");`. To get a response, you can use `string userInput = Console.ReadLine();`.

[Slide 4: File I/O]
- 📁 Moving beyond the console! File I/O allows your program to read from and write to files. It's like giving your program a notebook to store and retrieve information.

[Slide 5: Example - File I/O]
- 📝 Open the file cabinet! If you want to read from a text file, you can use `string content = File.ReadAllText("example.txt");`. To write to a file, you can use `File.WriteAllText("output.txt", "Hello, file world!");`.

[Slide 6: Exception Handling in I/O Operations]
- ⚠️ With great I/O power comes great responsibility! File operations can throw exceptions, especially when dealing with external resources. Be sure to handle exceptions gracefully to prevent crashes.

[Slide 7: Example - Exception Handling in File I/O]
- 🚨 Be prepared for surprises! If you're reading from a file, use a try-catch block to handle exceptions. For example:
```csharp
try
{
    string content = File.ReadAllText("nonexistent.txt");
    Console.WriteLine(content);
}
catch (FileNotFoundException)
{
    Console.WriteLine("File not found!");
}
```

[Slide 8: Stream I/O]
- 🌊 Enter the stream! Stream I/O provides a more versatile way to handle input and output, especially when dealing with large amounts of data or non-text files. It's like a flowing river of information.

[Slide 9: Example - Stream I/O]
- 🚣 Dive into the stream! If you're working with binary data, you can use `FileStream` to read and write bytes. For example:
```csharp
using (FileStream fs = new FileStream("binary.dat", FileMode.Create))
{
    byte[] data = { 1, 2, 3, 4, 5 };
    fs.Write(data, 0, data.Length);
}
```

[Slide 10: Benefits of I/O Operations]
- 🌈 I/O operations empower your programs to communicate, share information, and persist data. Whether it's interacting with users, reading from files, or dealing with streams, mastering I/O is a fundamental skill.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've embarked on the journey of I/O Operations in C#. Today, we covered Console I/O, File I/O, Stream I/O, and even touched on exception handling. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've gained the power to communicate and exchange information with I/O Operations in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Reading User Input

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're putting on our interactive hats and exploring the art of "Reading User Input" in C#. Get ready for a dynamic journey where your programs engage in conversations with users! 🎙️👩‍💻

[Slide 1: Importance of User Input]
- ➡️ User input is the heartbeat of interactive programs. It allows your applications to adapt, personalize, and engage users by capturing their responses. It's like turning your programs into responsive companions.

[Slide 2: Console.ReadLine()]
- 📚 Let's start with the basics! The workhorse for reading user input in the console world is `Console.ReadLine()`. It reads a line of text entered by the user and returns it as a string.

[Slide 3: Example - Console.ReadLine()]
- 🚀 Dive into the conversation! If you want to capture the user's name, you can use:
```csharp
Console.Write("Enter your name: ");
string userName = Console.ReadLine();
Console.WriteLine($"Hello, {userName}!");
```

[Slide 4: Reading Numeric Input]
- 🔢 What if you need numeric input? `Console.ReadLine()` returns a string, so you'll need to convert it to the desired numeric type using methods like `int.Parse()` or `Convert.ToInt32()`.

[Slide 5: Example - Reading Numeric Input]
- 🎯 Numeric quest! If you're expecting the user to enter their age, you can use:
```csharp
Console.Write("Enter your age: ");
string ageInput = Console.ReadLine();
int age = int.Parse(ageInput);
Console.WriteLine($"You are {age} years old.");
```

[Slide 6: Validating User Input]
- ⚖️ With great input comes great responsibility! Always validate user input to ensure it meets your program's expectations. Consider using methods like `int.TryParse()` for safer numeric conversions.

[Slide 7: Example - Validating User Input]
- 🛡️ Safety first! If you're expecting a numeric input, validate it like this:
```csharp
Console.Write("Enter your height (in cm): ");
string heightInput = Console.ReadLine();
if (int.TryParse(heightInput, out int height))
{
    Console.WriteLine($"Your height is {height} cm.");
}
else
{
    Console.WriteLine("Invalid input. Please enter a valid number.");
}
```

[Slide 8: Console.ReadKey()]
- 🎮 Sometimes, you want a single keypress instead of a whole line. Enter `Console.ReadKey()`, which captures a single keypress from the user.

[Slide 9: Example - Console.ReadKey()]
- 🕹️ Keymaster! If you want to capture a single key, you can use:
```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();
Console.WriteLine($"You pressed: {keyInfo.Key}");
```

[Slide 10: Benefits of Reading User Input]
- 🌈 Reading user input transforms your programs from monologues to dialogues. It enhances user experience, allows customization, and opens the door for user-driven interactions.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've mastered the art of "Reading User Input" in C#. Today, we covered `Console.ReadLine()`, reading numeric input, validating user input, and even a glimpse of `Console.ReadKey()`. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've unlocked the power to listen and respond to users with "Reading User Input" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Invalid Input

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're tackling the sometimes tricky territory of "Handling Invalid Input" in C#. Get ready to fortify your programs against unexpected user entries and ensure a smoother user experience! ⚔️🛡️

[Slide 1: The Challenge of Invalid Input]
- ➡️ Dealing with user input is like navigating a maze; you never know what users might enter. It's crucial to anticipate and handle invalid input gracefully to prevent crashes and create user-friendly applications.

[Slide 2: Common Sources of Invalid Input]
- 🚫 Invalid input can come from various sources: typos, incorrect data types, or unexpected user behavior. Your program needs to be resilient enough to handle these scenarios without breaking.

[Slide 3: Try-Catch Blocks for Exception Handling]
- 🕵️‍♂️ One powerful tool in your arsenal is the try-catch block. It allows you to catch and handle exceptions gracefully, preventing your program from crashing when faced with unexpected situations.

[Slide 4: Example - Basic Try-Catch Block]
- 🚨 Catch those exceptions! For example, when converting a string to an integer, you can use a try-catch block like this:
```csharp
try
{
    Console.Write("Enter a number: ");
    string userInput = Console.ReadLine();
    int number = int.Parse(userInput);
    Console.WriteLine($"You entered: {number}");
}
catch (FormatException)
{
    Console.WriteLine("Invalid input. Please enter a valid number.");
}
```

[Slide 5: Exception Types for Invalid Input]
- 📚 Different exceptions can occur based on the nature of invalid input. For example, `FormatException` is thrown when converting a string to a numeric type, and `OverflowException` can occur if the value is too large.

[Slide 6: Handling Multiple Exception Types]
- 🤹 Sometimes, you might encounter different types of exceptions. You can handle them in sequence by specifying multiple catch blocks. It's like having different nets to catch different types of fish.

[Slide 7: Example - Handling Multiple Exception Types]
- 🎭 Juggling exceptions! If you're converting a string to an integer or a double, you can handle both cases like this:
```csharp
try
{
    Console.Write("Enter a number: ");
    string userInput = Console.ReadLine();
    
    if (int.TryParse(userInput, out int intNumber))
    {
        Console.WriteLine($"You entered an integer: {intNumber}");
    }
    else if (double.TryParse(userInput, out double doubleNumber))
    {
        Console.WriteLine($"You entered a double: {doubleNumber}");
    }
    else
    {
        Console.WriteLine("Invalid input. Please enter a valid number.");
    }
}
catch (Exception ex)
{
    Console.WriteLine($"An error occurred: {ex.Message}");
}
```

[Slide 8: Customizing Error Messages]
- 🛠️ Make error messages user-friendly! Instead of showing generic messages, provide context-specific feedback to guide users on how to correct their input.

[Slide 9: Example - Customizing Error Messages]
- 🎨 Tailoring messages! If you expect a numeric input, guide the user with a custom error message:
```csharp
Console.Write("Enter your age: ");
string ageInput = Console.ReadLine();

if (int.TryParse(ageInput, out int age))
{
    Console.WriteLine($"You entered: {age}");
}
else
{
    Console.WriteLine("Invalid age. Please enter a valid number.");
}
```

[Slide 10: Benefits of Handling Invalid Input]
- 🌈 Handling invalid input is not just about preventing crashes; it's about creating a resilient and user-friendly experience. By guiding users and providing helpful feedback, you enhance the overall usability of your applications.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've fortified your programs against the unexpected with "Handling Invalid Input" in C#. Today, we explored try-catch blocks, different exception types, and customizing error messages. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've leveled up your programming resilience. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉

## Key Events

[Opening Slide]
- 🚀 Welcome back to the "C# Fundamentals" course! Today, we're tapping into the exciting realm of "Key Events" in C#. Get ready to capture the rhythm of user keystrokes and enhance the interactivity of your programs! 🎹👩‍💻

[Slide 1: The Power of Key Events]
- ➡️ Key events are like the musical notes of user interaction. They allow your programs to respond dynamically to each keystroke, opening the door to a world of possibilities in user interface design and gameplay.

[Slide 2: Console.ReadKey() Revisited]
- 🎮 Remember `Console.ReadKey()`? It's not just for single key captures; it can also be used to detect special keys and modifiers. It's like having a backstage pass to the concert of user input.

[Slide 3: Example - Console.ReadKey() with Special Keys]
- 🕹️ Special keys spotlight! If you want to detect arrow keys, you can use:
```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey(true); // true to suppress the key display
if (keyInfo.Key == ConsoleKey.UpArrow)
{
    Console.WriteLine("Up arrow key pressed!");
}
```

[Slide 4: ConsoleKey Enumeration]
- 🗝️ The `ConsoleKey` enumeration is your treasure map to the keyboard kingdom. It includes a variety of keys, from letters and numbers to function keys and modifiers.

[Slide 5: Example - ConsoleKey Enumeration]
- 🌐 Navigate the keys! If you want to check if the user pressed the Enter key, you can use:
```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();
if (keyInfo.Key == ConsoleKey.Enter)
{
    Console.WriteLine("Enter key pressed!");
}
```

[Slide 6: ConsoleModifiers]
- 🎭 Level up with modifiers! The `ConsoleModifiers` enumeration helps detect if the user is holding down additional keys like Shift or Control while pressing another key.

[Slide 7: Example - ConsoleModifiers]
- 🚀 Modifiers at play! If you want to check if the user pressed the letter 'A' with the Shift key held down, you can use:
```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();
if (keyInfo.Key == ConsoleKey.A && keyInfo.Modifiers == ConsoleModifiers.Shift)
{
    Console.WriteLine("Shift + A pressed!");
}
```

[Slide 8: Event-driven Key Events]
- 🚦 Enter the event-driven world! For more advanced scenarios and user interfaces, especially in graphical applications, you can leverage key events using frameworks like Windows Forms or WPF.

[Slide 9: Example - Event-driven Key Events (WPF)]
- 🌟 WPF magic! In a WPF application, you can handle key events like this:
```csharp
private void Window_KeyDown(object sender, KeyEventArgs e)
{
    if (e.Key == Key.A && (Keyboard.Modifiers & ModifierKeys.Control) == ModifierKeys.Control)
    {
        MessageBox.Show("Ctrl + A pressed!");
    }
}
```

[Slide 10: Benefits of Key Events]
- 🌈 Key events add a layer of dynamism to your applications. Whether you're creating games, interactive interfaces, or responding to hotkeys, mastering key events enhances user experience and engagement.

[Slide 11: Recap and Next Steps]
- 🎓 Bravo! You've unraveled the magic of "Key Events" in C#. Today, we explored `Console.ReadKey()`, the `ConsoleKey` enumeration, modifiers, and even peeked into event-driven key events. Join us in the upcoming modules for more coding adventures in the "C# Fundamentals" course.

[Closing Slide]
- 🚀 Congratulations! You've become the maestro of user interaction with "Key Events" in C#. Join us next time for more insights and hands-on coding adventures. Until then, happy coding! 🎉