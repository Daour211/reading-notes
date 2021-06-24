## Java Basics

## Variables:

- **Instance Variables (Non-Static Fields)**: Non-static fields are also known as instance variables because their values are unique to each instance of a class (to each object, in other words)

- **Class Variables (Static Fields)**: A class variable is any field declared with the static modifier; this tells the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated. The keyword final could be added to indicate that the number which we use will never change.

- **Local Variables**: The syntax for declaring a local variable is similar to declaring a field. There is no special keyword designating a variable as local; that determination comes entirely from the location in which the variable is declared

- **Parameters**: The important thing to remember is that parameters are always classified as "variables" not "fields"

**Naming**:

- Variable names are case-sensitive. A variable's name can be any legal identifier — an unlimited-length sequence of Unicode letters and digits, beginning with a letter, the dollar sign "$", or the underscore character "\_".<br>
  Additionally, the dollar sign character, by convention, is never used at all. A similar convention exists for the underscore character. White space is not permitted.

- Subsequent characters may be letters, digits, dollar signs, or underscore characters. Conventions (and common sense) apply to this rule as well. When choosing a name for your variables, use full words instead of cryptic abbreviations. Also keep in mind that the name you choose must not be a keyword or reserved word.

- If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word, capitalize the first letter of each subsequent word. If your variable stores a constant value, such as static final int NUM_GEARS = 6, the convention changes slightly, capitalizing every letter and separating subsequent words with the underscore character.

**Primitive Data Types:**

The Java programming language is statically-typed, which means that all variables must first be declared before they can be used

- **byte**: The byte data type is an 8-bit signed two's complement integer. It has a minimum value of -128 and a maximum value of 127 (inclusive). The byte data type can be useful for saving memory in large arrays.They can also be used in place of int where their limits help to clarify your code; the fact that a variable's range is limited can serve as a form of documentation.

- **short**: The short data type is a 16-bit signed two's complement integer. It has a minimum value of -32,768 and a maximum value of 32,767 (inclusive

- **int**: By default, the int data type is a 32-bit signed two's complement integer, which has a minimum value of -231 and a maximum value of 231-1. In Java SE 8 and later, you can use the int data type to represent an unsigned 32-bit integer, which has a minimum value of 0 and a maximum value of 232-1. Use the Integer class to use int data type as an unsigned integer

- **long**: The long data type is a 64-bit two's complement integer. The signed long has a minimum value of -263 and a maximum value of 263-1. In Java SE 8 and later, you can use the long data type to represent an unsigned 64-bit long, which has a minimum value of 0 and a maximum value of 264-1. Use this data type when you need a range of values wider than those provided by int.

- **float**: The float data type is a single-precision 32-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. As with the recommendations for byte and short, use a float (instead of double) if you need to save memory in large arrays of floating point numbers. This data type should never be used for precise values, such as currency

- **double**: The double data type is a double-precision 64-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. For decimal values, this data type is generally the default choice.
- boolean: The boolean data type has only two possible values: true and false. Use this data type for simple flags that track true/false conditions.

- **char**: The char data type is a single 16-bit Unicode character. It has a minimum value of '\u0000' (or 0) and a maximum value of '\uffff' (or 65,535 inclusive).

In addition to the eight primitive data types listed above, the Java programming language also provides special support for character strings via the java.lang.String class. Enclosing your character string within double quotes will automatically create a new String object; for example, String s = "this is a string";. String objects are immutable, which means that once created, their values cannot be changed. The String class is not technically a primitive data type, but considering the special support given to it by the language,

| DataType | efault Value (for fields) |
| -------- | ------------------------- |
| byte     | 0                         |
| short    | 0                         |
| int      | 0                         |
| long     | 0L                        |
| float    | 0.0f                      |
| double   | 0.0d                      |
| char     | '\u0000'                  |
| String   | null                      |
| boolean  | fasle                     |

**Literals**

A literal is the source code representation of a fixed value; literals are represented directly in your code without requiring computation. It's possible to assign a literal to a variable of a primitive type.

- **Integer Literals**

An integer literal is of type long if it ends with the letter L or l; otherwise it is of type int

Values of the integral types byte, short, int, and long can be created from int literals. Values of type long that exceed the range of int can be created from long literals. Integer literals can be expressed by these number systems:

• Decimal: Base 10, whose digits consists of the numbers 0 through 9; this is the number system you use every day
• Hexadecimal: Base 16, whose digits consist of the numbers 0 through 9 and the letters A through F
• Binary: Base 2, whose digits consists of the numbers 0 and 1 (you can create binary literals in Java SE 7 and later)

For general-purpose programming, the decimal system is likely to be the only number system you'll ever use. However, if you need to use another number system, the following example shows the correct syntax. The prefix 0x indicates hexadecimal and 0b indicates binary.

**Floating-Point Literals**
A floating-point literal is of type float if it ends with the letter F or f; otherwise its type is double and it can optionally end with the letter D or d.

The floating point types (float and double) can also be expressed using E or e (for scientific notation). F or f (32-bit float literal) and D or d (64-bit double literal; this is the default and by convention is omitted).

example:
double d1 = 123.4;
// same value as d1, but in scientific notation
double d2 = 1.234e2;
float f1 = 123.4f;

**Character and String Literals**
Literals of types char and String may contain any Unicode (UTF-16) characters. If your editor and file system does not allow it, you can use a "Unicode escape" such as '\u0108' (capital C with circumflex).
Unicode escape sequences may be used elsewhere in a program (such as in field names, for example), not just in char or String literals.
**Always use 'single quotes' for char literals and "double quotes" for String literals**

The Java programming language also supports a few special escape sequences for char and String literals: \b (backspace), \t (tab), \n (line feed), \f (form feed), \r (carriage return), \" (double quote), \' (single quote), and \\ (backslash).
There's also a special null literal that can be used as a value for any reference type. null may be assigned to any variable, except variables of primitive types. There's little you can do with a null value beyond testing for its presence. Therefore, null is often used in programs as a marker to indicate that some object is unavailable.

**Using Underscore Characters in Numeric Literals**

if your code contains numbers with many digits, you can use an underscore character to separate digits in groups of three, similar to how you would use a punctuation mark like a comma, or a space, as a separator.
You can place underscores only between digits; you cannot place underscores in the following places:

• At the beginning or end of a number
• Adjacent to a decimal point in a floating point literal
• Prior to an F or L suffix
• In positions where a string of digits is expected

### Arrays:

An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed.

**Declaring a Variable to Refer to an Array:**

An array declaration has two components: the array's type and the array's name. An array's type is written as type[], where type is the data type of the contained elements; the brackets are special symbols indicating that this variable holds an array. As with variables of other types, the declaration does not actually create an array; it simply tells the compiler that this variable will hold an array of the specified type.

**Creating, Initializing, and Accessing an Array**

- One way to create an array is with the **new** operator.

- you can use the shortcut syntax to create and initialize an array

- You can also declare an array of arrays (also known as a **multidimensional array**) by using two or more sets of brackets, such as String[][] names. Each element, therefore, must be accessed by a corresponding number of index values.
  In the Java programming language, a multidimensional array is an array whose components are themselves arrays

**Copying Arrays**

The System class has an **arraycopy** method that you can use to efficiently copy data from one array into another.
The two Object arguments specify the array to copy from and the array to copy to. The three int arguments specify the starting position in the source array, the starting position in the destination array, and the number of array elements to copy.

**Array Manipulations**

Java SE provides several methods for performing array manipulations (common tasks, such as copying, sorting and searching arrays) in the java.util.Arrays class
The difference between **copyOfRange** & **arraycopy**is that using the copyOfRange method does not require you to create the destination array before calling the method, because the destination array is returned by the method.

Some other useful operations provided by methods in the java.util.Arrays class are:

- Searching an array for a specific value to get the index at which it is placed (the binarySearch method).

- Comparing two arrays to determine if they are equal or not (the equals method).

- Filling an array to place a specific value at each index (the fill method).

- Sorting an array into ascending order. This can be done either sequentially, using the sort method, or concurrently, using the parallelSort method introduced in Java SE 8. Parallel sorting of large arrays on multiprocessor systems is faster than sequential array sorting.

- Creating a stream that uses an array as its source (the stream method).

- Converting an array to a string. The toString method converts each element of the array to a string, separates them with commas, then surrounds them with brackets

## Operators

Operators are special symbols that perform specific operations on one, two, or three operands, and then return a result.

The operators in the following table are listed according to precedence order. The closer to the top of the table an operator appears, the higher its precedence.

When operators of equal precedence appear in the same expression, a rule must govern which is evaluated first. All binary operators except for the assignment operators are evaluated from left to right; assignment operators are evaluated right to left.

Operator Precedence

| Operators         | efault Precedence             |
| ----------------- | ----------------------------- |
| postfix           | expr++ expr--                 |
| unary             | ++expr --expr +expr -expr ~ ! |
| multiplicative    | \_ / %                        |
| additive          | + -                           |
| shift             | << >> >>>                     |
| relational        | < > <= >= instanceof          |
| equality          | == !=                         |
| bitwise           | AND &                         |
| bitwise exclusive | OR ^                          |
| bitwise inclusive | OR                            |
| logical AND       | AND &&                        |
| logical OR        | OR                            |
| ternary           | ? :                           |

<!-- | assignment        | = += -= \_= /= %= &= ^= |= <<= >>= >>>= | -->

**Assignment, Arithmetic, and Unary Operators**
The Simple Assignment Operator: One of the most common operators that you'll encounter is the simple assignment operator "=". This operator can also be used on objects to assign object references.

**The Arithmetic Operators**

| Operators | Description             |
| --------- | ----------------------- |
| +         | Additive operator       |
| -         | Subtraction operator    |
| \*        | Multiplication operator |
| /         | Division operator       |
| %         | Remainder operator      |

- The + operator can also be used for concatenating (joining) two strings together.

The Unary Operators
The unary operators require only one operand; they perform various operations such as incrementing/decrementing a value by one, negating an expression, or inverting the value of a boolean.

| Operators | Description                                                                                |
| --------- | ------------------------------------------------------------------------------------------ |
| +         | Unary plus operator; indicates positive value (numbers are positive without this, however) |
| -         | Unary minus operator; negates an expression                                                |
| ++        | Increment operator; increments a value by 1                                                |
| --        | Decrement operator; decrements a value by 1                                                |
| !         | Logical complement operator; inverts the value of a boolean                                |

The increment/decrement operators can be applied before **(prefix)** or after **(postfix)** the operand. The code result++; and ++result; will both end in result being incremented by one. **The only difference is that the prefix version (++result) evaluates to the incremented value, whereas the postfix version (result++) evaluates to the original value**. If you are just performing a simple increment/decrement, it doesn't really matter which version you choose. But if you use this operator in part of a larger expression, the one that you choose may make a significant difference.

**Equality, Relational, and Conditional Operators**

The Equality and Relational Operators

| Operators | Description              |
| --------- | ------------------------ |
| ==        | equal to                 |
| !=        | not equal to             |
| >         | greater than             |
| >=        | greater than or equal to |
| <         | less than                |
| <=        | less than or equal to    |

**The Conditional Operators**

The **&&** and **||** operators perform Conditional-AND and Conditional-OR operations on two boolean expressions. These operators exhibit "short-circuiting" behavior, which means that the second operand is evaluated only if needed.

**The Type Comparison Operator instanceof**

The **instanceof** operator compares an object to a specified type. You can use it to test if an object is an instance of a class, an instance of a subclass, or an instance of a class that implements a particular interface.

**Bitwise and Bit Shift Operators**

The Java programming language also provides operators that perform bitwise and bit shift operations on integral types.
The unary bitwise complement operator "~" inverts a bit pattern; it can be applied to any of the integral types, making every "0" a "1" and every "1" a "0".

The signed left shift operator "<<" shifts a bit pattern to the left, and the signed right shift operator ">>" shifts a bit pattern to the right. The bit pattern is given by the left-hand operand, and the number of positions to shift by the right-hand operand. The unsigned right shift operator ">>>" shifts a zero into the leftmost position, while the leftmost position after ">>" depends on sign extension.

The bitwise & operator performs a bitwise AND operation.

The bitwise ^ operator performs a bitwise exclusive OR operation.

The bitwise | operator performs a bitwise inclusive OR operation.

### Expressions, Statements, and Blocks

**Expressions**

An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.
The data type of the value returned by an expression depends on the elements used in the expression

**Statements**

Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution
The following types of expressions can be made into a statement by terminating the expression with a semicolon (;).

• Assignment expressions<br>
• Any use of ++ or --<br>
• Method invocations<br>
• Object creation expressions

In addition to expression statements, there are two other kinds of statements: declaration statements and control flow statements. A declaration statement declares a variable.

Finally, control flow statements regulate the order in which statements get executed.

**Blocks**

A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

### Control Flow Statements

The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code.

The decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return)

**The if-then and if-then-else Statements**

1-**The if-then Statement**

The if-then statement is the most basic of all the control flow statements. It tells your program to execute a certain section of code only if a particular test evaluates to true

2- **The if-then-else Statement**

The if-then-else statement provides a secondary path of execution when an "if" clause evaluates to false.

**The switch Statement**

The switch statement can have a number of possible execution paths. A switch works with the byte, short, char, and int primitive data types. It also works with enumerated types (discussed in Enum Types), the String class, and a few special classes that wrap certain primitive types: Character, Byte, Short, and Integer

The body of a switch statement is known as a switch block. A statement in the switch block can be labeled with one or more case or default labels. The switch statement evaluates its expression, then executes all statements that follow the matching case label.

- **Deciding whether to use if-then-else statements or a switch statement is based on readability and the expression that the statement is testing. An if-then-else statement can test expressions based on ranges of values or conditions, whereas a switch statement tests expressions based only on a single integer, enumerated value, or String object.**

**Using Strings in switch Statements**
In Java SE 7 and later, you can use a String object in the switch statement's expression.

**The while and do-while Statements**

The while statement continually executes a block of statements while a particular condition is true. <br>
**The difference between do-while and while is that do-while evaluates its expression at the bottom of the loop instead of the top. Therefore, the statements within the do block are always executed at least once.**

**The for Statement**

The for statement provides a compact way to iterate over a range of values.

**Branching Statements**
1-**The break Statement:**

The break statement has two forms: labeled and unlabeled.

The unlabeled form in the previous discussion of the switch statement. You can also use an unlabeled break to terminate a for, while, or do-while loop

An unlabeled break statement terminates the innermost switch, for, while, or do-while statement, but a labeled break terminates an outer statement.

The break statement terminates the labeled statement; it does not transfer the flow of control to the label. Control flow is transferred to the statement immediately following the labeled (terminated) statement.

2-**The continue Statement**

The continue statement skips the current iteration of a for, while , or do-while loop. The unlabeled form skips to the end of the innermost loop's body and evaluates the boolean expression that controls the loop.
A labeled continue statement skips the current iteration of an outer loop marked with the given label.

3-**The return Statement**
The return statement exits from the current method, and control flow returns to where the method was invoked. The return statement has two forms: one that returns a value, and one that doesn't.

# The first response in this Reddit thread on compiling

## What does it mean to compile code?

The compiler (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable.

You may run into is people saying code does or does not compile. This means the compilor they used checks to make sure their program is written correctly according to the rules of the programming language

# Reading Java Documentation

I can search for a thing reading the Java through its API. And I have more than one way to search for what I want.

**Searching for a term**

You can find things in the API documentation in a number of different ways. Each way is convenient in one situation or another.

1- Using the index
2- Using the list of classes

**Resources**:

- [Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

- [The first response in this Reddit thread on compiling](https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)

- [XKCD: Compiling](https://xkcd.com/303/)

- [Reading Java Documentation](https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/)
