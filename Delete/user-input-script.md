# User Input
### 1. **Introduction to User Input:**
   - **Overview:**
     - User input is a fundamental aspect of interactive software. It allows programs to receive data or instructions from users during runtime, enhancing the versatility and dynamism of applications.

### 2. **Standard Input and Output Streams:**
   - **Console Class in C#:**
     - In C#, the `Console` class provides a streamlined mechanism for interacting with the standard input (`Console.In`) and output (`Console.Out`) streams.

   - **C# Example:**
   ```csharp
   Console.Write("Enter your name: ");
   string userName = Console.ReadLine();
   Console.WriteLine($"Hello, {userName}!");
   ```

### 3. **Reading Different Data Types:**
   - **Parsing User Input:**
     - The `Console.ReadLine()` method returns user input as a string. To work with other data types, parsing is required.

   - **C# Example:**
   ```csharp
   Console.Write("Enter your age: ");
   int userAge = int.Parse(Console.ReadLine());
   ```

### 4. **Input Validation:**
   - **Handling Invalid Input:**
     - Input validation is crucial to ensure the program responds gracefully to unexpected user input. Techniques like `int.TryParse()` can be employed.

   - **C# Example:**
   ```csharp
   Console.Write("Enter a number: ");
   string userInput = Console.ReadLine();

   if (int.TryParse(userInput, out int result))
   {
       Console.WriteLine($"You entered: {result}");
   }
   else
   {
       Console.WriteLine("Invalid input. Please enter a valid number.");
   }
   ```

### 5. **Console Class Methods:**
   - **Additional Console Methods:**
     - The `Console` class offers various methods for formatted output, clearing the console, and more.

   - **C# Example:**
   ```csharp
   Console.WriteLine("This is a formatted number: {0:N2}", 1234.5678);
   Console.Clear(); // Clears the console screen
   ```

### 6. **Key Events and Console.ReadKey():**
   - **Detecting Key Press Events:**
     - The `Console.ReadKey()` method allows capturing key events, enabling more interactive console applications.

   - **C# Example:**
   ```csharp
   ConsoleKeyInfo keyInfo = Console.ReadKey();
   Console.WriteLine($"Key pressed: {keyInfo.KeyChar}");
   ```

### 7. **Command-Line Arguments:**
   - **Passing Arguments to Programs:**
     - Command-line arguments provide a means to pass parameters to a C# program during execution.

   - **C# Example:**
   ```csharp
   static void Main(string[] args)
   {
       Console.WriteLine($"Number of command-line arguments: {args.Length}");
       foreach (var arg in args)
       {
           Console.WriteLine($"Argument: {arg}");
       }
   }
   ```

### 8. **Conclusion:**
   - **Incorporating User Input:**
     - Effectively integrating user input mechanisms enhances the interactivity and usability of C# applications. Employing the `Console` class and related methods enables developers to create dynamic and responsive programs, fostering a more engaging user experience.
