# C# OOP
## Introduction to C# Object-Oriented Programming (OOP) Course

Welcome to the C# Object-Oriented Programming (OOP) Course – a comprehensive guide crafted to elevate your proficiency in C# development. This chapter introduces the course structure, outlines the objectives, and provides a glimpse into the fundamental concepts that form the backbone of this journey.
### 1.1 Course Objectives
  Understand OOP Fundamentals: Delve into the foundational principles of OOP, such as encapsulation, inheritance, and polymorphism, and discover their application in C#.
  Apply Design Patterns: Learn to implement common design patterns, enabling you to tackle real-world problems with efficiency and maintainability.
  Utilize C# Features: Explore the rich feature set of C#, including properties, events, delegates, and LINQ, to empower your ability to build robust applications.
  Develop Industry-Standard Practices: Embrace best practices in C# development, ensuring your code is organized, error-resistant, and easily maintainable.

### 1.2 Prerequisites

This course is designed for individuals with a basic understanding of programming concepts and familiarity with C# syntax. Whether you are a beginner or an experienced developer, the content caters to a wide audience looking to enhance their skills in object-oriented programming with C#.
<hr>

## Introduction to Object-Oriented Programming (OOP)
### 1. Overview

In this chapter, we explore the fundamental principles of Object-Oriented Programming (OOP) within the context of C#. A comprehensive understanding of OOP is crucial for developing software applications with a focus on scalability and robustness.
### 2. Understanding Object-Oriented Programming (OOP)
#### 2.1 Definition

Object-Oriented Programming (OOP) is centered around the concept of "objects," where an object encapsulates data and behavior. This approach provides a structured and modular framework for software design.
#### 2.2 Key Concepts
##### 2.2.1 Classes and Objects

A class serves as a blueprint defining the structure and behavior of objects. Objects, which are instances of classes, represent tangible entities in software.

Example:

``` csharp

class Car
{
    public string Model { get; set; }
    public void StartEngine()
    {
        Console.WriteLine("Engine started!");
    }
}

Car myCar = new Car();
myCar.Model = "Sedan";
myCar.Color = "Blue";
myCar.StartEngine();
```

##### 2.2.2 Encapsulation

Encapsulation involves bundling data (attributes) and methods (functions) into a single unit, typically a class. This helps in concealing internal complexities, emphasizing essential features.

##### 2.2.3 Inheritance

Inheritance allows a class to inherit properties and behavior from another class, promoting code reuse and establishing a hierarchical relationship.

**Example:**
```csharp
class Animal
{
    public void Eat()
    {
        Console.WriteLine("Eating...");
    }
}

class Dog : Animal
{
    public void Bark()
    {
        Console.WriteLine("Woof!");
    }
}

Dog myDog = new Dog();
myDog.Eat();  // Inherited from Animal
myDog.Bark();
```

##### 2.2.4 Polymorphism

Polymorphism enables treating objects of different types as objects of a common base type, fostering flexibility and extensibility.

**Example:**
```csharp
class Shape
{
    public virtual void Draw()
    {
        Console.WriteLine("Drawing a shape...");
    }
}

class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}

class Square : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a square...");
    }
}

Shape myShape = new Circle();
myShape.Draw();  // Calls the overridden method in Circle class
```

### 3. Benefits of Object-Oriented Programming in C#

#### 3.1 Code Reusability

OOP promotes code reuse through features like inheritance, enabling developers to build upon existing classes and extend functionality.

#### 3.2 Modularity

Encapsulation of data and behavior into classes enhances modularity, simplifying maintenance and promoting a clear organizational structure.
#### 3.3 Flexibility and Extensibility

The principles of polymorphism and inheritance in OOP provide flexibility in code design. This flexibility allows for the creation of adaptable systems that can evolve and scale as project requirements change.

#### 3.4 Improved Maintenance

The modular nature of OOP facilitates easier maintenance. Changes to one part of the code (a class or an object) do not necessarily impact other parts, reducing the risk of unintended consequences and streamlining the maintenance process.

### 4. C# Application of OOP Concepts

C# is a powerful programming language that embraces and extends the principles of OOP. The language's syntax and features align seamlessly with OOP concepts, allowing developers to implement robust and scalable applications.

#### 4.1 Defining Classes in C#

In C#, classes are defined using a straightforward syntax. Attributes (data) and methods (behavior) are encapsulated within the class structure.

**Example:**
```csharp
class Student
{
    public string Name { get; set; }
    public int Age { get; set; }

    public void Study()
    {
        Console.WriteLine("Studying...");
    }
}

Student myStudent = new Student();
myStudent.Name = "John Doe";
myStudent.Age = 20;
myStudent.Study();
```

#### 4.2 Implementing Inheritance in C#

C# supports inheritance, allowing one class to inherit properties and behavior from another. This feature enhances code organization and facilitates code reuse.

**Example:**
```csharp
class Animal
{
    public void Eat()
    {
        Console.WriteLine("Eating...");
    }
}

class Dog : Animal
{
    public void Bark()
    {
        Console.WriteLine("Woof!");
    }
}

Dog myDog = new Dog();
myDog.Eat();  // Inherited from Animal
myDog.Bark();
```

#### 4.3 Applying Polymorphism in C#

Polymorphism in C# enables the use of objects of different types through a common interface. This allows for the creation of flexible and extensible systems.

**Example:**
```csharp
class Shape
{
    public virtual void Draw()
    {
        Console.WriteLine("Drawing a shape...");
    }
}

class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}

class Square : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a square...");
    }
}

Shape myShape = new Circle();
myShape.Draw();  // Calls the overridden method in Circle class
```

### 5. Conclusion
In conclusion, this chapter has provided an in-depth introduction to Object-Oriented Programming (OOP) concepts in the context of C#. Understanding these principles is fundamental to building scalable, modular, and maintainable software applications. As we proceed through the course, these foundational concepts will serve as the bedrock for more advanced topics and practical applications in C# OOP development.
<hr>

## Struct in C#

### 1. Overview

This chapter explores the concept of `struct` in C#, a value type that represents a lightweight alternative to classes. Understanding the use cases and behavior of `structs` is essential for efficient memory management and performance optimization.

### 2. What is a Struct?

A `struct` is a value type in C# that encapsulates data and related functionalities. Unlike classes, which are reference types, `structs` are value types, meaning they store their data directly where they are declared, leading to more efficient memory usage.

### 3. Key Characteristics of Structs

#### 3.1 Value Type Semantics

`structs` exhibit value type semantics, meaning when assigned to a new variable or passed as a method parameter, a copy of the entire struct is made. This is in contrast to reference types, where variables reference the same object.

#### 3.2 Default Parameterless Constructor

Unlike classes, `structs` do not have a default parameterless constructor provided by the compiler. If needed, developers must explicitly define their constructors.

### 4. When to Use Structs

#### 4.1 Lightweight Data Structures

Use `structs` for lightweight data structures that primarily encapsulate a small set of data without complex behaviors. Examples include representing a point in 2D space or a color.

**Example:**
```csharp
public struct Point
{
    public int X;
    public int Y;

    public Point(int x, int y)
    {
        X = x;
        Y = y;
    }
}

// Usage
Point myPoint = new Point(10, 20);
```

#### 4.2 Performance Considerations

Consider using `structs` in scenarios where memory allocation overhead needs to be minimized. `structs` can be beneficial for performance-critical operations.

### 5. Limitations of Structs

#### 5.1 Immutability

`structs` are generally immutable. Once a `struct` instance is created, its properties cannot be modified individually. If modification is required, a new instance must be created.

#### 5.2 Size Limitation

Due to their value type nature, large or complex `structs` may result in performance degradation and increased memory usage. In such cases, classes might be a more suitable choice.

### 6. Guidelines for Using Structs

#### 6.1 Keep it Simple

Design simple `structs` with minimal data and behavior to maintain their efficiency and fulfill their intended purpose as lightweight data containers.

#### 6.2 Prefer Immutability

Design `structs` to be immutable where possible. Immutability ensures predictable behavior and eliminates concerns related to unexpected modifications.

### 7. Conclusion

Understanding the role and limitations of `structs` in C# is crucial for making informed design decisions. While `structs` offer performance benefits for certain scenarios, it's essential to apply them judiciously, considering their limitations and adhering to best practices in software design. As we progress through the course, we'll explore practical examples and use cases to solidify our understanding of the `struct` type in C#.

<hr>

## Enum
### 1. Overview

This chapter introduces the concept of `enum` in C#, a powerful and concise way to define a set of named integral constants. Understanding `enums` is essential for enhancing code readability and maintainability when working with predefined sets of values.

### 2. What is an Enum?

An `enum` (enumeration) in C# is a value type that defines a set of named integral constants. It provides a more expressive and readable way to represent fixed sets of values, making code more self-documenting and less error-prone.

### 3. Declaration and Syntax

#### 3.1 Basic Enum Declaration

An `enum` is declared using the `enum` keyword, followed by the enumeration name and a set of named constants enclosed in curly braces.

**Example:**
```csharp
public enum DaysOfWeek
{
    Sunday,
    Monday,
    Tuesday,
    Wednesday,
    Thursday,
    Friday,
    Saturday
}
```

#### 3.2 Assigning Custom Values

Constants in an `enum` are assigned default integer values starting from 0. Custom values can be assigned explicitly, and subsequent constants continue from the last assigned value.

**Example:**
```csharp
public enum Months
{
    January = 1,
    February,
    March,
    April,
    May,
    June,
    July,
    August,
    September,
    October,
    November,
    December
}
```

### 4. Enum Underlying Type

The underlying type of an `enum` is implicitly `int` by default. However, it can be explicitly specified using a different integral type such as `byte`, `short`, or `long`.

**Example:**
```csharp
public enum Status : byte
{
    Inactive,
    Active
}
```

### 5. Use Cases and Benefits

#### 5.1 Improved Readability

`enums` enhance code readability by providing meaningful names to integral constants, making the code more self-explanatory.

#### 5.2 Preventing Magic Numbers

Instead of using "magic numbers" in the code, `enums` offer named constants, reducing the risk of errors and improving code maintainability.

**Example:**
```csharp
// Without Enum
if (status == 1)
{
    // Code logic for active status
}

// With Enum
if (status == Status.Active)
{
    // Code logic for active status
}
```

#### 5.3 Switch Statements

`enums` are commonly used in switch statements, improving code structure and reducing the likelihood of mistakes.

**Example:**
```csharp
switch (day)
{
    case DaysOfWeek.Saturday:
    case DaysOfWeek.Sunday:
        Console.WriteLine("It's the weekend!");
        break;
    default:
        Console.WriteLine("It's a weekday.");
        break;
}
```

### 6. Enumerating Enums

#### 6.1 Obtaining Enum Names and Values

The `Enum` class in C# provides methods to retrieve the names and values of the constants defined in an `enum`.

**Example:**
```csharp
string[] dayNames = Enum.GetNames(typeof(DaysOfWeek));
int[] dayValues = (int[])Enum.GetValues(typeof(DaysOfWeek));
```

#### 6.2 Parsing Enum Values

The `Enum` class allows parsing strings into enum values, providing a flexible way to convert user inputs.

**Example:**
```csharp
DaysOfWeek parsedDay;
if (Enum.TryParse("Monday", out parsedDay))
{
    Console.WriteLine($"Parsed Day: {parsedDay}");
}
```

### 7. Conclusion
In conclusion, the `enum` type in C# offers a concise and expressive way to represent sets of named constants. Leveraging `enums` improves code readability, reduces the use of magic numbers, and enhances the maintainability of the codebase. As we progress through the course, we'll explore practical examples and scenarios where `enums` prove to be a valuable tool in C# development.

<hr>

## Encapsulation
### 1. Overview

This chapter delves into the fundamental concept of encapsulation in C#. Encapsulation is a key principle of Object-Oriented Programming (OOP) that involves bundling data and methods that operate on the data into a single unit, promoting modularity and data protection.

### 2. What is Encapsulation?

Encapsulation is the concept of bundling the data (attributes) and methods (functions) that operate on the data into a single unit known as a class. This unit acts as a protective container, controlling the access to the internal components and exposing only what is necessary.

### 3. Key Features of Encapsulation

#### 3.1 Access Modifiers

Encapsulation utilizes access modifiers such as `public`, `private`, and `protected` to control the visibility of class members. This ensures that certain data and methods are only accessible within the class itself or by specific external entities.

**Example:**
```csharp
public class BankAccount
{
    private decimal balance;

    public void Deposit(decimal amount)
    {
        // Accessible within the class
        balance += amount;
    }

    public decimal GetBalance()
    {
        // Accessible within the class
        return balance;
    }
}
```

#### 3.2 Properties and Methods

Encapsulation involves the use of properties to encapsulate data and methods to encapsulate behavior. Properties provide controlled access to the internal state of the class, and methods perform operations on that state.

**Example:**
```csharp
public class Person
{
    private string name;

    public string Name
    {
        get { return name; }
        set
        {
            // Additional logic can be added here
            name = value;
        }
    }

    public void DisplayInformation()
    {
        // Accessible within the class
        Console.WriteLine($"Name: {name}");
    }
}
```

### 4. Benefits of Encapsulation

#### 4.1 Data Protection

Encapsulation shields the internal state of a class from direct external manipulation. This prevents unintended modifications and ensures that data integrity is maintained.

#### 4.2 Modularity

By bundling related data and methods together, encapsulation promotes modularity. Each class becomes a self-contained unit, making the code more organized and easier to maintain.

#### 4.3 Code Flexibility

Encapsulation allows developers to modify the internal implementation of a class without affecting the external code that uses the class. This flexibility is crucial for evolving and maintaining large codebases.

### 5. Best Practices for Encapsulation

#### 5.1 Use Properties for Data Access

Properties provide a controlled interface for accessing and modifying the internal state of a class. Utilize properties to encapsulate data and ensure proper validation and encapsulation.

#### 5.2 Limit Exposure of Internal State

Minimize the use of `public` access modifiers and expose only what is necessary for external interaction. This prevents unintended manipulation of internal state.

### 6. Encapsulation in Real-world Scenarios

#### 6.1 Database Connection Example

Encapsulation is evident in scenarios like database connections, where the internal details of establishing a connection are encapsulated within a class, exposing only essential methods for interaction.

**Example:**
```csharp
public class DatabaseConnection
{
    private SqlConnection connection;

    public void OpenConnection(string connectionString)
    {
        // Encapsulated logic to establish a connection
        connection = new SqlConnection(connectionString);
        connection.Open();
    }

    public void CloseConnection()
    {
        // Encapsulated logic to close the connection
        connection.Close();
    }
}
```

### 7. Conclusion
Encapsulation is a fundamental principle in C# that enhances code organization, data protection, and flexibility. Understanding and applying encapsulation is essential for building maintainable and scalable software. As we progress through the course, we'll explore how encapsulation integrates with other OOP concepts to create robust and modular C# applications.
<hr>

## Inheritance Object
### 1. Overview

This chapter explores the concept of inheritance in C#, a powerful mechanism that allows a class to inherit properties and behaviors from another class. Understanding inheritance is crucial for building reusable and extensible code.

### 2. What is Inheritance?

Inheritance is a key concept in Object-Oriented Programming (OOP) that enables a class, known as the derived or child class, to inherit properties and behaviors from another class, known as the base or parent class. This promotes code reuse and establishes a hierarchical relationship between classes.

### 3. Basic Syntax of Inheritance

#### 3.1 Base Class Declaration

A base class contains the common properties and methods shared by one or more derived classes. It is declared using the `class` keyword.

**Example:**
```csharp
public class Animal
{
    public void Eat()
    {
        Console.WriteLine("Eating...");
    }
}
```

#### 3.2 Derived Class Declaration

A derived class inherits from a base class using the `:` syntax. It gains access to the properties and methods of the base class and can extend or override them.

**Example:**
```csharp
public class Dog : Animal
{
    public void Bark()
    {
        Console.WriteLine("Woof!");
    }
}
```

### 4. Access Modifiers in Inheritance

#### 4.1 Public Access

Public members of the base class are accessible in the derived class. This includes public methods, properties, and fields.

**Example:**
```csharp
public class Shape
{
    public void Draw()
    {
        Console.WriteLine("Drawing...");
    }
}

public class Circle : Shape
{
    // Inherits Draw method from Shape
}
```

#### 4.2 Protected Access

Protected members of the base class are accessible in the derived class but not directly accessible outside the class hierarchy.

**Example:**
```csharp
public class Vehicle
{
    protected void StartEngine()
    {
        Console.WriteLine("Engine started...");
    }
}

public class Car : Vehicle
{
    public void Drive()
    {
        // Can access StartEngine
        StartEngine();
        Console.WriteLine("Car is moving...");
    }
}
```

### 5. Overriding and Extending Methods

#### 5.1 Overriding Methods

A derived class can override a method from the base class to provide a specialized implementation. This is achieved using the `override` keyword.

**Example:**
```csharp
public class Shape
{
    public virtual void Draw()
    {
        Console.WriteLine("Drawing a shape...");
    }
}

public class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}
```

#### 5.2 Extending Methods

In addition to overriding, a derived class can extend a method by calling the base class's implementation using the `base` keyword.

**Example:**
```csharp
public class Vehicle
{
    public virtual void Start()
    {
        Console.WriteLine("Vehicle started...");
    }
}

public class Car : Vehicle
{
    public override void Start()
    {
        base.Start(); // Call the base class's Start method
        Console.WriteLine("Car started...");
    }
}
```

### 6. Using Base Class Constructors

A derived class can use the constructor of the base class using the `base` keyword to initialize base class-specific members.

**Example:**
```csharp
public class Person
{
    public string Name { get; set; }

    public Person(string name)
    {
        Name = name;
    }
}

public class Employee : Person
{
    public string Role { get; set; }

    public Employee(string name, string role) : base(name)
    {
        Role = role;
    }
}
```

### 7. Conclusion
Inheritance is a powerful mechanism in C# that promotes code reuse and establishes relationships between classes. Understanding how to use inheritance effectively is essential for creating well-organized, extensible, and maintainable codebases. As we progress through the course, we'll explore advanced concepts and practical examples that leverage the benefits of inheritance in C#.
<hr>

## Abstraction
### 1. Overview

This chapter explores the concept of abstraction in C#, an essential principle of Object-Oriented Programming (OOP). Abstraction allows developers to model complex systems by focusing on relevant details while hiding unnecessary complexities.

### 2. What is Abstraction?

Abstraction is the process of simplifying complex systems by representing only the essential features and hiding unnecessary details. In C#, abstraction is implemented through abstract classes, interfaces, and abstract methods.

### 3. Abstract Classes

#### 3.1 Declaring Abstract Classes

An abstract class is a class that cannot be instantiated on its own and may contain abstract methods. Abstract methods are declared without an implementation in the abstract class and must be implemented by derived (non-abstract) classes.

**Example:**
```csharp
public abstract class Shape
{
    public abstract void Draw();
}

public class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}
```

#### 3.2 Abstract Properties and Methods

In addition to methods, abstract classes can have abstract properties, providing a blueprint for derived classes to implement.

**Example:**
```csharp
public abstract class Animal
{
    public abstract string Sound { get; }

    public abstract void MakeSound();
}

public class Dog : Animal
{
    public override string Sound => "Woof";

    public override void MakeSound()
    {
        Console.WriteLine("Woof! Woof!");
    }
}
```

### 4. Interfaces

#### 4.1 Defining Interfaces

An interface is a contract that defines a set of methods and properties. Classes implementing an interface must provide concrete implementations for all the members defined in the interface.

**Example:**
```csharp
public interface ILogger
{
    void Log(string message);
}

public class ConsoleLogger : ILogger
{
    public void Log(string message)
    {
        Console.WriteLine($"Logging: {message}");
    }
}
```

#### 4.2 Multiple Interface Implementation

A class in C# can implement multiple interfaces, allowing it to conform to multiple contracts.

**Example:**
```csharp
public interface IEmailSender
{
    void SendEmail(string to, string subject, string body);
}

public class NotificationService : ILogger, IEmailSender
{
    public void Log(string message)
    {
        Console.WriteLine($"Logging: {message}");
    }

    public void SendEmail(string to, string subject, string body)
    {
        Console.WriteLine($"Sending email to {to} with subject '{subject}': {body}");
    }
}
```

### 5. Benefits of Abstraction

#### 5.1 Code Reusability

Abstraction promotes code reuse by defining common structures that can be implemented by multiple classes.

#### 5.2 Maintainability

By focusing on essential features and hiding implementation details, abstraction enhances code maintainability. Changes to the internal details of a class do not impact its external usage.

#### 5.3 Flexibility

Abstraction allows for flexibility in designing systems. New classes can be introduced without affecting existing code, provided they adhere to the defined abstract classes or interfaces.

### 6. Conclusion

Abstraction is a crucial concept in C# that enables developers to create flexible, maintainable, and reusable code. Abstract classes and interfaces provide powerful tools for modeling complex systems while managing complexity. As we progress through the course, we'll explore advanced abstraction techniques and practical applications in C# development.
<hr>

## Polymorphism
### 1. Overview

This chapter explores the concept of polymorphism in C#, a fundamental principle of Object-Oriented Programming (OOP). Polymorphism allows objects of different types to be treated as objects of a common base type, promoting flexibility and extensibility in code.

### 2. What is Polymorphism?

Polymorphism, derived from the Greek words "poly" (many) and "morph" (form), refers to the ability of objects to take on multiple forms. In C#, polymorphism allows a single interface or base class to represent various types and to provide a common interface for interacting with objects of different types.

### 3. Types of Polymorphism

#### 3.1 Compile-Time Polymorphism (Static Binding)

Compile-time polymorphism, also known as static binding, occurs when the method or operation to be called is determined at compile time. This is achieved through method overloading and operator overloading.

##### Example: Method Overloading
```csharp
public class Calculator
{
    public int Add(int a, int b)
    {
        return a + b;
    }

    public double Add(double a, double b)
    {
        return a + b;
    }
}
```

#### 3.2 Runtime Polymorphism (Dynamic Binding)

Runtime polymorphism, also known as dynamic binding or late binding, occurs when the method or operation to be called is determined at runtime. This is achieved through method overriding and interfaces.

##### Example: Method Overriding
```csharp
public class Shape
{
    public virtual void Draw()
    {
        Console.WriteLine("Drawing a shape...");
    }
}

public class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}
```

### 4. Method Overriding and Virtual Methods

#### 4.1 Defining Virtual Methods

In C#, the `virtual` keyword is used to declare a method in a base class that can be overridden by derived classes. This allows for dynamic dispatch of the method at runtime.

##### Example: Virtual Method
```csharp
public class Animal
{
    public virtual void MakeSound()
    {
        Console.WriteLine("Animal makes a sound...");
    }
}

public class Dog : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Dog barks...");
    }
}
```

#### 4.2 Using `base` Keyword in Overrides

The `base` keyword is used in derived class methods to explicitly call the overridden method in the base class.

##### Example: Using `base` Keyword
```csharp
public class Vehicle
{
    public virtual void Start()
    {
        Console.WriteLine("Vehicle started...");
    }
}

public class Car : Vehicle
{
    public override void Start()
    {
        base.Start(); // Call the base class's Start method
        Console.WriteLine("Car started...");
    }
}
```

### 5. Interfaces and Polymorphism

#### 5.1 Implementing Interfaces

Polymorphism is achieved through interfaces by allowing multiple classes to implement a common set of methods, providing a consistent interface.

##### Example: Interface
```csharp
public interface ILogger
{
    void Log(string message);
}

public class ConsoleLogger : ILogger
{
    public void Log(string message)
    {
        Console.WriteLine($"Logging: {message}");
    }
}
```

#### 5.2 Using Polymorphism with Interfaces

Classes that implement an interface can be treated as instances of that interface, allowing for polymorphic behavior.

##### Example: Polymorphism with Interface
```csharp
ILogger logger = new ConsoleLogger();
logger.Log("Log this message");
```

### 6. Benefits of Polymorphism

#### 6.1 Code Flexibility

Polymorphism provides code flexibility by allowing objects of different types to be treated as objects of a common base type or interface.

#### 6.2 Code Extensibility

New classes can be introduced without modifying existing code, as long as they adhere to the common interface or base type.

#### 6.3 Dynamic Behavior

Polymorphism enables dynamic behavior, where the actual method or operation called is determined at runtime based on the type of the object.

### 7. Conclusion

Polymorphism is a powerful concept in C# that enhances code flexibility and extensibility. By allowing objects to be treated in a more general way, polymorphism contributes to creating more adaptable and maintainable software. As we progress through the course, we'll explore advanced polymorphic scenarios and practical applications in C# development.
<hr>

## Operators Overloading
### 1. Overview

This chapter explores the concept of operator overloading in C#, a feature that allows developers to redefine the behavior of operators for user-defined types. Operator overloading provides flexibility and expressiveness in working with custom classes.

### 2. What is Operator Overloading?

Operator overloading allows developers to redefine the behavior of operators for user-defined types. In C#, certain operators can be overloaded to work with custom classes, providing a more natural and intuitive syntax for operations on those classes.

### 3. Overloadable Operators

#### 3.1 Common Overloadable Operators

Some common overloadable operators in C# include `+`, `-`, `*`, `/` for arithmetic operations, `==`, `!=`, `<`, `>` for comparison, `++`, `--` for increment and decrement, and more.

#### 3.2 Example: Overloading the `+` Operator

```csharp
public class ComplexNumber
{
    public double Real { get; set; }
    public double Imaginary { get; set; }

    public ComplexNumber(double real, double imaginary)
    {
        Real = real;
        Imaginary = imaginary;
    }

    // Overloading the + operator
    public static ComplexNumber operator +(ComplexNumber a, ComplexNumber b)
    {
        return new ComplexNumber(a.Real + b.Real, a.Imaginary + b.Imaginary);
    }
}

// Usage
ComplexNumber num1 = new ComplexNumber(2, 3);
ComplexNumber num2 = new ComplexNumber(1, 4);
ComplexNumber sum = num1 + num2;
```

### 4. Guidelines for Operator Overloading

#### 4.1 Overloading Unary Operators

Unary operators like `+`, `-`, `++`, `--` can be overloaded by defining corresponding methods in the class.

#### 4.2 Overloading Binary Operators

Binary operators like `+`, `-`, `*`, `/` can be overloaded by defining corresponding methods with the `operator` keyword.

#### 4.3 Consistency in Overloading

Maintain consistency in the behavior of overloaded operators to avoid confusion for developers using the class.

#### 4.4 Avoid Overloading Core Operators

Avoid overloading core operators to ensure code readability and prevent unexpected behavior.

### 5. Example: Overloading Equality Operators

```csharp
public class Person
{
    public string Name { get; set; }
    public int Age { get; set; }

    // Overloading the == operator
    public static bool operator ==(Person person1, Person person2)
    {
        return person1?.Name == person2?.Name && person1?.Age == person2?.Age;
    }

    // Overloading the != operator
    public static bool operator !=(Person person1, Person person2)
    {
        return !(person1 == person2);
    }
}

// Usage
Person person1 = new Person { Name = "John", Age = 30 };
Person person2 = new Person { Name = "John", Age = 30 };
bool areEqual = person1 == person2; // true
```

### 6. Conclusion
Operator overloading in C# is a powerful feature that allows developers to redefine the behavior of operators for user-defined types. While it provides flexibility and expressiveness, it should be used judiciously to maintain code readability and consistency. As we progress through the course, we'll explore more advanced scenarios and practical applications of operator overloading in C# development.
<hr>

## Extension Methods
### 1. Overview

This chapter explores the concept of extension methods in C#, a powerful feature that allows developers to add new methods to existing types without modifying their source code. Extension methods enhance code readability and reusability.

### 2. What are Extension Methods?

Extension methods are a way to add new methods to existing types without modifying their source code. They are defined in static classes and must be static methods, making them a powerful tool for extending the functionality of classes, even those defined in third-party libraries.

### 3. Defining Extension Methods

#### 3.1 Syntax for Extension Methods

Extension methods are defined as static methods within a static class. The first parameter of the method specifies the type being extended using the `this` keyword.

```csharp
public static class StringExtensions
{
    public static string Reverse(this string input)
    {
        char[] charArray = input.ToCharArray();
        Array.Reverse(charArray);
        return new string(charArray);
    }
}

// Usage
string original = "Hello";
string reversed = original.Reverse(); // "olleH"
```

#### 3.2 Limitations of Extension Methods

Extension methods cannot access private members of the extended type, and they cannot override existing methods in the extended type.

### 4. Guidelines for Extension Methods

#### 4.1 Naming Conventions

Use meaningful names for extension methods that clearly indicate their purpose.

#### 4.2 Targeting Specific Types

Consider the context and target specific types for which the extension method makes sense.

#### 4.3 Organizing Extension Methods

Organize extension methods into logically grouped static classes to enhance code organization.

### 5. Real-world Example: LINQ Extension Methods

```csharp
public static class EnumerableExtensions
{
    public static IEnumerable<T> CustomWhere<T>(this IEnumerable<T> source, Func<T, bool> predicate)
    {
        foreach (var item in source)
        {
            if (predicate(item))
            {
                yield return item;
            }
        }
    }

    public static IEnumerable<TResult> CustomSelect<T, TResult>(this IEnumerable<T> source, Func<T, TResult> selector)
    {
        foreach (var item in source)
        {
            yield return selector(item);
        }
    }
}

// Usage
var numbers = new List<int> { 1, 2, 3, 4, 5 };
var evenNumbers = numbers.CustomWhere(n => n % 2 == 0);
var squaredNumbers = numbers.CustomSelect(n => n * n);
```

### 6. Extension Methods and Code Readability

Extension methods can significantly enhance code readability by allowing developers to write expressive and fluent code.

```csharp
var result = "Hello, Extension Methods!".Reverse().ToUpper();
```

### 7. Conclusion

Extension methods in C# provide a flexible and readable way to extend the functionality of existing types. While they should be used judiciously and adhere to naming conventions, extension methods can significantly improve code organization and expressiveness. As we progress through the course, we'll explore more advanced scenarios and practical applications of extension methods in C# development.
<hr>

## Generics
### 1. Overview

This chapter explores the concept of generics in C#, a powerful feature that allows developers to create classes, methods, and structures with placeholder types. Generics provide flexibility and type safety in a wide range of scenarios.

### 2. What are Generics?

Generics in C# allow you to write classes, methods, and structures with placeholders for data types. These placeholders, known as type parameters, enable the creation of reusable and type-safe components that work with a variety of data types.

### 3. Generic Classes

#### 3.1 Declaring Generic Classes

A generic class is declared using the `<T>` syntax, where `T` is the type parameter.

```csharp
public class Box<T>
{
    public T Content { get; set; }

    public Box(T content)
    {
        Content = content;
    }
}

// Usage
Box<int> intBox = new Box<int>(42);
Box<string> stringBox = new Box<string>("Hello, Generics!");
```

#### 3.2 Constraints on Type Parameters

Constraints can be applied to type parameters to restrict them to certain types or to require that they implement specific interfaces.

```csharp
public class Calculator<T> where T : struct
{
    public T Add(T a, T b)
    {
        return (dynamic)a + b;
    }
}
```

### 4. Generic Methods

#### 4.1 Declaring Generic Methods

A generic method is declared similarly to a generic class, with the `<T>` syntax indicating the type parameter.

```csharp
public static T GetFirst<T>(T[] array)
{
    if (array.Length > 0)
    {
        return array[0];
    }
    throw new InvalidOperationException("Array is empty");
}
```

#### 4.2 Inference of Type Arguments

Type inference allows the compiler to deduce the type arguments based on the method's usage.

```csharp
int[] numbers = { 1, 2, 3, 4, 5 };
int firstNumber = GetFirst(numbers); // Type inference infers T as int
```

### 5. Generic Interfaces and Delegates

#### 5.1 Generic Interfaces

Interfaces can be defined with generic type parameters, providing flexibility in implementing various data types.

```csharp
public interface IRepository<T>
{
    void Save(T entity);
    T GetById(int id);
}
```

#### 5.2 Generic Delegates

Delegates can also be generic, allowing the definition of functions that work with different types.

```csharp
public delegate TResult Transformer<T, TResult>(T input);
```

### 6. Benefits of Generics

#### 6.1 Code Reusability

Generics promote code reusability by creating components that can work with multiple data types.

#### 6.2 Type Safety

Generics provide type safety, reducing the likelihood of runtime errors by catching type mismatches at compile-time.

#### 6.3 Performance

Generics offer better performance compared to non-generic alternatives, as they avoid the need for boxing and unboxing operations.

### 7. Real-world Example: Generic Collections

```csharp
List<int> numbers = new List<int> { 1, 2, 3, 4, 5 };
Dictionary<string, int> dictionary = new Dictionary<string, int>();
Queue<double> queue = new Queue<double>();
```

### 8. Conclusion
Generics in C# are a powerful feature that enhances code reusability, type safety, and performance. Whether used in classes, methods, interfaces, or delegates, generics provide a flexible and efficient way to write code that works with a variety of data types. As we progress through the course, we'll explore more advanced scenarios and practical applications of generics in C# development.
<hr>

## Reflection API
### 1. Overview

This chapter explores the Reflection API in C#, a powerful feature that allows developers to inspect and interact with types, methods, properties, and other members of assemblies at runtime. Reflection provides dynamic access to object information, making it useful for various scenarios such as serialization, code analysis, and dependency injection.

### 2. What is Reflection?

Reflection is the ability of a program to inspect its own structure, types, and members at runtime. In C#, the Reflection API provides classes and methods to dynamically examine and interact with the metadata of types and assemblies.

### 3. Key Components of Reflection

#### 3.1 `System.Reflection` Namespace

The `System.Reflection` namespace contains classes and interfaces that enable reflection in C#. Key classes include `Assembly`, `Type`, `MethodInfo`, `PropertyInfo`, and more.

#### 3.2 `Type` Class

The `Type` class represents a type and provides methods to retrieve information about the type, such as its methods, properties, fields, and events.

#### 3.3 `Assembly` Class

The `Assembly` class represents an assembly and provides methods to access information about the types contained within the assembly.

### 4. Common Reflection Scenarios

#### 4.1 Inspecting Types

```csharp
Type myType = typeof(MyClass);
MethodInfo[] methods = myType.GetMethods();
```

#### 4.2 Creating Instances Dynamically

```csharp
Type myType = typeof(MyClass);
object instance = Activator.CreateInstance(myType);
```

#### 4.3 Invoking Methods

```csharp
Type myType = typeof(MyClass);
MethodInfo method = myType.GetMethod("MyMethod");
object result = method.Invoke(instance, parameters);
```

#### 4.4 Accessing Properties

```csharp
Type myType = typeof(MyClass);
PropertyInfo property = myType.GetProperty("MyProperty");
object value = property.GetValue(instance);
```

#### 4.5 Working with Attributes

```csharp
Type myType = typeof(MyClass);
MyAttribute attribute = (MyAttribute)Attribute.GetCustomAttribute(myType, typeof(MyAttribute));
```

### 5. Real-world Example: Dependency Injection with Reflection

```csharp
public class DependencyInjector
{
    public T Resolve<T>()
    {
        Type targetType = typeof(T);
        // Logic to resolve and create an instance
        return (T)Activator.CreateInstance(targetType);
    }
}
```

### 6. Benefits of Reflection

#### 6.1 Dynamic Code Analysis

Reflection allows dynamic analysis of code structures, enabling scenarios such as unit testing frameworks, code generators, and serialization/deserialization.

#### 6.2 Dependency Injection

Reflection is often used in dependency injection containers to dynamically resolve and instantiate dependencies.

#### 6.3 Frameworks and Libraries

Many frameworks and libraries leverage reflection to provide generic and extensible functionality, such as object mapping, serialization, and aspect-oriented programming.

### 7. Challenges and Considerations

#### 7.1 Performance Overhead

Reflection can have performance overhead compared to static code due to its dynamic nature. It's important to use it judiciously in performance-critical scenarios.

#### 7.2 Lack of Compile-time Safety

Reflection operates at runtime, and errors related to types and members may only be discovered at runtime, reducing compile-time safety.

### 8. Conclusion
Reflection in C# is a powerful feature that provides dynamic access to type information at runtime. While it offers flexibility and extensibility, developers should use it carefully, considering performance implications and potential lack of compile-time safety. As we progress through the course, we'll explore more advanced scenarios and practical applications of reflection in C# development.
<hr>

## Design Patterns
### 1. Overview

This chapter introduces Design Patterns in C#, a set of proven solutions to recurring design problems in software development. Design Patterns provide a common vocabulary and best practices that help in creating maintainable, scalable, and flexible software.

### 2. What are Design Patterns?

Design Patterns are reusable solutions to common problems encountered in software design. They represent best practices that have evolved over time and provide a shared vocabulary for developers. Design Patterns are not blueprints or templates; instead, they guide developers on how to structure their code to solve specific problems.

### 3. Categories of Design Patterns

#### 3.1 Creational Patterns

Creational patterns deal with the process of object creation. They abstract the instantiation process, making the system independent of how its objects are created, composed, and represented.

- **Singleton Pattern:** Ensures a class has only one instance and provides a global point of access to it.

```csharp
public class Singleton
{
    private static Singleton instance;

    private Singleton() { }

    public static Singleton Instance
    {
        get
        {
            if (instance == null)
            {
                instance = new Singleton();
            }
            return instance;
        }
    }
}
```

- **Factory Method Pattern:** Defines an interface for creating an object but leaves the choice of its type to the subclasses, creating an instance of the appropriate subclass.

```csharp
public abstract class Creator
{
    public abstract Product FactoryMethod();
}

public class ConcreteCreatorA : Creator
{
    public override Product FactoryMethod()
    {
        return new ConcreteProductA();
    }
}

public class ConcreteCreatorB : Creator
{
    public override Product FactoryMethod()
    {
        return new ConcreteProductB();
    }
}
```

#### 3.2 Structural Patterns

Structural patterns focus on how classes and objects are composed to form larger structures.

- **Adapter Pattern:** Allows the interface of an existing class to be used as another interface.

```csharp
public class Adaptee
{
    public void SpecificRequest()
    {
        Console.WriteLine("Specific request");
    }
}

public interface ITarget
{
    void Request();
}

public class Adapter : ITarget
{
    private readonly Adaptee adaptee;

    public Adapter(Adaptee adaptee)
    {
        this.adaptee = adaptee;
    }

    public void Request()
    {
        adaptee.SpecificRequest();
    }
}
```

- **Decorator Pattern:** Attaches additional responsibilities to an object dynamically.

```csharp
public interface IComponent
{
    void Operation();
}

public class ConcreteComponent : IComponent
{
    public void Operation()
    {
        Console.WriteLine("ConcreteComponent operation");
    }
}

public class Decorator : IComponent
{
    private readonly IComponent component;

    public Decorator(IComponent component)
    {
        this.component = component;
    }

    public void Operation()
    {
        component.Operation();
    }
}
```

#### 3.3 Behavioral Patterns

Behavioral patterns define algorithms and communication patterns between objects.

- **Observer Pattern:** Defines a one-to-many dependency between objects, so that when one object changes state, all its dependents are notified and updated automatically.

```csharp
public interface IObserver
{
    void Update(string message);
}

public class ConcreteObserver : IObserver
{
    private readonly string name;

    public ConcreteObserver(string name)
    {
        this.name = name;
    }

    public void Update(string message)
    {
        Console.WriteLine($"{name} received the message: {message}");
    }
}

public interface ISubject
{
    void Attach(IObserver observer);
    void Detach(IObserver observer);
    void Notify(string message);
}

public class ConcreteSubject : ISubject
{
    private readonly List<IObserver> observers = new List<IObserver>();

    public void Attach(IObserver observer)
    {
        observers.Add(observer);
    }

    public void Detach(IObserver observer)
    {
        observers.Remove(observer);
    }

    public void Notify(string message)
    {
        foreach (var observer in observers)
        {
            observer.Update(message);
        }
    }
}
```

- **Strategy Pattern:** Defines a family of algorithms, encapsulates each algorithm, and makes them interchangeable.

```csharp
public interface IStrategy
{
    void Execute();
}

public class ConcreteStrategyA : IStrategy
{
    public void Execute()
    {
        Console.WriteLine("Executing strategy A");
    }
}

public class ConcreteStrategyB : IStrategy
{
    public void Execute()
    {
        Console.WriteLine("Executing strategy B");
    }
}

public class Context
{
    private IStrategy strategy;

    public void SetStrategy(IStrategy strategy)
    {
        this.strategy = strategy;
    }

    public void ExecuteStrategy()
    {
        strategy.Execute();
    }
}
```

### 4. Benefits of Design Patterns

#### 4.1 Reusability

Design Patterns promote reusability by providing proven solutions to common problems, reducing the need to reinvent the wheel.

#### 4.2 Maintainability

Using Design Patterns leads to more maintainable code as they provide a clear structure and a common language for developers.

#### 4.3 Flexibility

Design Patterns enhance the flexibility of a codebase, making it easier to adapt to changing requirements.

### 5. Real-world Example: MVC Pattern

The Model-View-Controller (MVC) pattern separates an application into three interconnected components: the model (data and business logic), the view (user interface), and the controller (handles user input and updates the model).

### 6. Conclusion

Design Patterns are essential tools in a software developer's toolkit. They provide solutions to common design problems and offer a shared vocabulary for communication among developers. By understanding and applying Design Patterns, developers can create maintainable, scalable, and flexible software solutions. As we progress through the course, we'll explore more advanced Design Patterns and practical applications in C# development.
<hr>

## Anonymous types
### 1. Overview

This chapter introduces the concept of Anonymous Types in C#, a feature that allows developers to create simple, read-only types on-the-fly without explicitly defining a class. Anonymous types are often used in scenarios where a quick and disposable type is needed for a specific purpose.

### 2. What are Anonymous Types?

Anonymous Types in C# are a way to create simple, read-only types without explicitly defining a class. They are particularly useful in scenarios where a temporary, short-lived type is needed, such as during LINQ queries or when returning multiple values from a method.

### 3. Creating Anonymous Types

Anonymous types are created using the `new` keyword and an object initializer syntax. The compiler automatically infers the type based on the properties specified in the initialization.

```csharp
var person = new { FirstName = "John", LastName = "Doe", Age = 30 };
```

In this example, `person` is an anonymous type with properties `FirstName`, `LastName`, and `Age`. The type is inferred by the compiler.

### 4. Usage in LINQ Queries

Anonymous types are commonly used in LINQ queries to project data into a new shape.

```csharp
var employees = new List<Employee>
{
    new Employee { FirstName = "Alice", LastName = "Smith", Salary = 50000 },
    new Employee { FirstName = "Bob", LastName = "Johnson", Salary = 60000 },
    // ...
};

var query = from employee in employees
            select new { employee.FirstName, employee.LastName, AnnualBonus = employee.Salary * 0.1 };

foreach (var result in query)
{
    Console.WriteLine($"{result.FirstName} {result.LastName}, Bonus: {result.AnnualBonus}");
}
```

In this example, the LINQ query projects the data into an anonymous type with properties `FirstName`, `LastName`, and `AnnualBonus`.

### 5. Limitations of Anonymous Types

#### 5.1 Read-Only Properties

Properties of anonymous types are read-only, meaning you can't modify their values after initialization.

#### 5.2 Limited Use Cases

Anonymous types are suitable for scenarios where a short-lived type is needed, but they are not a replacement for named types in all situations.

### 6. Real-world Example: Data Projection

```csharp
var orders = new List<Order>
{
    new Order { ProductName = "Laptop", Quantity = 2, Price = 1200 },
    new Order { ProductName = "Monitor", Quantity = 1, Price = 300 },
    // ...
};

var orderSummary = orders.Select(order => new { order.ProductName, TotalCost = order.Quantity * order.Price });

foreach (var summary in orderSummary)
{
    Console.WriteLine($"Product: {summary.ProductName}, Total Cost: {summary.TotalCost}");
}
```

In this example, the `orderSummary` projection uses an anonymous type to calculate and display the total cost of each product.

### 7. Conclusion

Anonymous Types in C# provide a concise and convenient way to create simple, read-only types on-the-fly. They are particularly useful in scenarios like LINQ queries where a temporary and disposable type is needed. However, it's essential to be aware of their limitations and use them appropriately in the context of their intended purpose. As we progress through the course, we'll explore more language features and their practical applications in C# development.
<hr>
