### Enhanced Console-Based Calculator

This is a console-based calculator created in Java that supports basic arithmetic, scientific functions, and unit conversions. It is a menu-driven application that allows the user to switch between a scientific calculator and a unit converter, built with a focus on modularity and robust error handling.

### Features

#### Main Menu
A user-friendly main menu allows for navigation between the calculator's core functions:
* Scientific Calculator
* Unit Converter
* Exit

#### Scientific Calculator
The scientific calculator mode supports both binary and unary operations. Users can perform a calculation and immediately enter another one in a continuous loop.
* **Binary Operations**: Addition (`+`), Subtraction (`-`), Multiplication (`*`), Division (`/`), and Power (`pow`).
* **Unary Operations**: Square Root (`sqrt`), Sine (`sin`), Cosine (`cos`), Tangent (`tan`), Natural Log (`log`), and Base-10 Log (`log10`).
* **Trigonometric Handling**: Automatically converts degree-based input to radians for `sin`, `cos`, and `tan` functions using `Math.toRadians()`.
* **Zero Division Check**: Prevents runtime errors by explicitly checking for and flagging division by zero.

#### Unit Converter
The unit converter has its own sub-menu for different categories of conversions.
* **Temperature Conversion**: Converts values between Celsius ('C'), Fahrenheit ('F'), and Kelvin ('K').
* **Currency Conversion**: Converts between USD, EUR, and INR using pre-defined fixed exchange rates.
* **Weight Conversion**: Converts values between Kilograms ('kg'), Grams ('g'), Pounds ('lb'), and Ounces ('oz').

### Technical Implementation

This project was built to demonstrate proficiency in core Java concepts and software design principles.
* **State Management**: The application flow is managed by a `ProgramState` enum, creating a simple and effective finite-state machine to switch between menus and modules.
* **Modular Design**: The codebase is organized into distinct, single-responsibility methods (e.g., `runScientificCalculator()`, `convertTemperature()`, `convertCurrency()`) for improved readability, maintainability, and organization.
* **Error Handling**: Invalid user inputs are managed gracefully using `try-catch` blocks to handle exceptions like `InputMismatchException`. This prevents application crashes and provides helpful, color-coded error messages to the user.
* **User-Friendly Console**: ANSI escape codes are used to add color to the console output, differentiating prompts (`ANSI_YELLOW`), results (`ANSI_GREEN`), and error messages (`ANSI_RED`) for a clearer and more engaging user experience.

### Skills Demonstrated

This project covers several key programming skills:
* Java Fundamentals & Math Logic
* Control Flow (Conditionals and Loops)
* Modular Programming (Methods)
* Input/Output Handling (`Scanner`)
* Robust Error and Exception Handling
