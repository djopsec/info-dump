# Glossary for Programming Basics

## A
**algorithm**  
A finite set of well-defined instructions used to solve a problem or perform a task. Algorithms are the heart of programming—whether you're sorting data, finding the shortest path, or calculating results.

**argument**  
A value you pass to a function when calling it. Arguments are inputs that influence how a function behaves. Example: in `greet("Soft")`, `"Soft"` is the argument.

**array**  
A fixed-size data structure that holds elements of the same type in a specific order, accessible via an index. Languages like Java and C use arrays more rigidly than Python (which uses lists).

**assignment operator (`=`)**  
Used to assign the value on the right to the variable on the left. Example: `x = 5` stores the number 5 in the variable `x`.

**attribute**  
A variable attached to an object. For example, a `Car` object might have attributes like `color` and `speed`. Attributes help define the state of an object.

**autocompletion**  
A code editor feature that predicts what you want to type, saving time and reducing typos. It can suggest variable names, functions, methods, and more.

---

## B
**block**  
A group of code statements that are treated as a unit. In Python, blocks are defined by indentation; in other languages, they're usually enclosed in braces `{}`.

**bug**  
An error in the code that causes unexpected behavior or incorrect results. Debugging is the process of identifying and fixing bugs.

---

## C
**class**  
A blueprint for creating objects (a particular data structure). Classes encapsulate data (attributes) and behavior (methods). Used heavily in object-oriented programming (OOP).

**collection**  
A data structure that stores multiple values, like lists, dictionaries, arrays, or sets. Useful for managing groups of related items.

**comment**  
A line in the code not executed by the computer, used to explain what the code does. Good commenting helps with code readability and collaboration.

**comment out**  
Temporarily disabling code by converting it into a comment. Helps test different parts of code without deleting anything.

**compile**  
The process of converting source code into machine code. Languages like C or Java are compiled before running. Python, however, is interpreted.

**concatenation**  
Joining two or more strings together. Example: `"Hello, " + "world!"` results in `"Hello, world!"`.

**concise**  
Clear and brief code that accomplishes a task in as few lines as possible, without sacrificing readability.

**conditional expression**  
An expression that evaluates to `True` or `False`. Used in decision-making structures like `if` statements.

**constructor function**  
A special function used to initialize objects from a class. In Python, this is the `__init__` method.

**crash**  
When a program stops unexpectedly, often due to runtime errors like division by zero or accessing an invalid index.

---

## D
**data type**  
Describes what kind of value a variable can hold (e.g., integer, string, float). Understanding data types helps you write correct and efficient code.

**debug**  
To identify and fix bugs or problems in a program. Modern IDEs and debuggers let you step through code, inspect variables, and monitor execution.

**dictionary (collection)**  
Stores key-value pairs. Keys must be unique. Example: `{"name": "Soft", "role": "developer"}`. Useful for fast lookups and grouping related data.

---

## E
**expression**  
Any combination of variables, values, and operators that evaluates to a single result. Example: `2 + 3 * x` is an expression.

---

## F
**field**  
Another term for an object’s attribute or property. Example: `user.name` accesses the `name` field of a user object.

**file extension**  
Indicates the file’s type or purpose. Common extensions: `.py` for Python, `.js` for JavaScript, `.html` for HTML documents.

**float**  
A number with a decimal point. Example: `3.14`. Floating-point arithmetic can be tricky due to precision issues.

**for loop**  
Executes a block of code a specific number of times or once for each item in a collection. Example:  
```python
for name in names:
    print(name)
```

**framework**  
A collection of libraries and tools to help build applications faster. Examples: Django for web apps, PyTest for testing.

**function**  
A reusable block of code that performs a specific task. Encourages modular, organized, and DRY (Don’t Repeat Yourself) code.

**function body**  
The indented or bracketed code inside a function. It runs when the function is called.

**function call**  
Executes a function by name and passes arguments. Example: `print("Hello")` is a function call.

---

## G
**garbage collection**  
The process of automatically freeing memory that a program no longer uses. Languages like Python handle this behind the scenes.

**gutter**  
The space beside your code in an IDE where line numbers and breakpoints appear.

---

## H
**high-level language**  
Languages that are closer to human language and abstract away hardware details. Easier to read and write than low-level code (e.g., assembly).

---

## I
**IDE (Integrated Development Environment)**  
A software suite for programming that includes a code editor, compiler/interpreter, debugger, and other tools. Examples: VS Code, PyCharm.

**if-else statement**  
Controls program flow based on a condition. Example:
```python
if x > 10:
    print("Big number")
else:
    print("Small number")
```

**if statement**  
Executes code only if the condition is true.

**immutable**  
Cannot be changed once created. Tuples and strings in Python are immutable. Helps with safer, more predictable code.

**importing**  
Pulling in external code (modules or libraries) to use in your own program. Example: `import math`

**index / index number**  
The position of an item in a list or array. Python uses zero-based indexing (`my_list[0]` is the first item).

**infinite loop**  
A loop that never ends, often by mistake. Can crash programs or consume all resources.

**integer**  
A whole number without a decimal. Example: `5`, `-2`.

**IntelliSense**  
Microsoft’s code-suggestion tool in Visual Studio Code. Helps reduce syntax errors and speed up development.

**interpret**  
To run code line-by-line, translating as it goes. Languages like Python and JavaScript are interpreted.

**int method**  
Converts a string or float to an integer. Example: `int("42")` → `42`.

**IO (Input/Output)**  
Describes communication between a program and the outside world. Examples: `input()` in Python, file writing, or printing output.

**iterate**  
Loop through each item in a collection. For example, `for i in range(5)` iterates five times.

---

## K
**keyword**  
A reserved word in a programming language that has a special meaning. You can’t use these as variable names. Examples: `if`, `while`, `return`.

---

## L
**linting**  
Analyzes code for potential errors or bad practices before runtime. Tools like `pylint` or `flake8` help enforce code quality.

**list (collection)**  
An ordered collection of items that can be modified. Example: `["apple", "banana", "cherry"]`

**loop**  
A control structure that repeats code until a condition is met. Can be a `for` or `while` loop.

---

## M
**machine language**  
The binary (0s and 1s) code that computers execute directly. Human-readable languages are eventually compiled or interpreted into this.

**method**  
A function associated with an object or class. Example: `"hello".upper()` calls the `upper` method on a string.

**module**  
A file containing Python code, such as functions and classes, that can be imported into other programs.

**multi-threading**  
Running multiple tasks simultaneously in one program. Useful for I/O-bound processes like downloading multiple files at once.

**mutable**  
Can be changed after creation. Lists are mutable, meaning you can add or remove elements.

---

## O
**object-oriented programming (OOP)**  
A paradigm that structures programs using objects—bundles of data and methods. Encourages reusability, modularity, and abstraction.

**operand**  
A value used with an operator. In `4 + 3`, the operands are `4` and `3`.

**operator**  
A symbol that performs operations on operands. Arithmetic (`+`, `-`), logical (`and`, `or`), comparison (`==`, `!=`) are common.

**order of operations**  
The sequence used to evaluate expressions. Follows math rules: parentheses, exponents, multiplication/division, addition/subtraction (PEMDAS).

---

## P
**package**  
A directory of related modules. Python uses `pip` to install packages like `numpy` or `requests`.

**parameter**  
A variable used in a function definition to accept arguments. Example: `def greet(name):` — `name` is a parameter.

**PEP 8**  
The official Python style guide that promotes readability and consistent coding practices.

**programming**  
The process of designing and writing instructions a computer can follow to perform tasks or solve problems.

**property**  
A way to control access to an object’s data, usually with getter/setter methods in OOP.

**pseudocode**  
A simplified, language-agnostic way to express program logic. Useful for planning before coding.

---

## R
**regular expression**  
A tool for matching patterns in text using a specific syntax. Example: `r"\d+"` matches one or more digits.

**relational operator**  
Compares values: `==`, `!=`, `>`, `<`, `>=`, `<=`. Returns a Boolean result.

**return value**  
The result a function gives back when it finishes. Use `return` to send values out of a function.

**runtime error**  
An error that occurs while the program is running, like trying to divide by zero or access an invalid list index.

---

## S
**semantic error**  
A logical error where the program runs but doesn’t behave as intended. Example: using `+` when you meant to use `*`.

**slice**  
A portion of a list or string. Syntax: `list[start:end]`. Python makes slicing simple and powerful.

**source code**  
The human-readable instructions written by a programmer, saved in files like `.py`, `.js`, or `.java`.

**statement**  
A complete instruction that performs some action. Example: `x = 10` is a statement.

**style guide**  
A document defining coding standards for readability, naming conventions, and structure. Promotes consistency across teams.

**syntax**  
The set of rules that defines how code must be written for the computer to understand it.

**syntax error**  
An error in code structure that prevents the program from running. Example: missing a colon in an `if` statement.

**syntax highlighting**  
Color-coding in code editors that improves readability by distinguishing keywords, strings, functions, and variables.

---

## T
**test case**  
A set of inputs and expected outputs used to check if a function or program works correctly. Used in unit testing.

**tuple**  
An ordered, immutable sequence of values. Useful for grouping data you don’t want to change.

---

## V
**variable**  
A named container that holds a value. Can be changed during the program's execution unless declared `const` or immutable.

---

## W
**while loop**  
Repeats a block of code as long as a condition remains true. Be careful to ensure the condition will eventually become false.

**white space**  
Spaces, tabs, and blank lines used to format code. In Python, indentation (a type of whitespace) is syntactically significant.
