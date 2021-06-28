## Java Primitives versus Objects

### Java Type System:

There are two-fold type system in Java:

- Primitives: int, boolean
- reference types: Integer, Boolean.

**Wrapper classes (reference type)** are immutable which means that their state can't change when the object is constructed, and it cannot be inherited from them” final”

**Autoboxing** is the process of converting a primitive type to a reference one

**Unboxing** is the process of converting a reference one to primitive type

### Pros and Cons

**Single Item Memory Footprint**

The primitive type variables have impact on the memory:

- boolean – 1 bit
- byte – 8 bits
- short, char – 16 bits
- int, float – 32 bits
- long, double – 64 bits

* **The primitive type variables in the stack which considered relatively fast to get**
* **The reference type are objects in the heap which considered relatively slow to get**

The reference type variables have impact on the memory:

- Boolean – 128 bits
- Byte – 128 bits
- Short, Character – 128 bits
- Integer, Float – 128 bits
- Long, Double – 192 bits

**Memory Footprint for Arrays**

The arrays take much more space in the memory and also depends on the size of the array.
Size with respect to how the memory m(s) depends on the number of elements s of the array:

- long, double: m(s) = 128 + 64 s
- short, char: m(s) = 128 + 64 [s/4]
- byte, boolean: m(s) = 128 + 64 [s/8]
- the rest: m(s) = 128 + 64 [s/2]

**Performance**

The performance of Java code depends on many things, but one of them which we mentioned earlier important is what type we are using (primitive or reference) which will determine where they will be saved.

**Usage**

The use pf primitive type is more preferable but in the current Java there are some restrictions which must be taken in consideration to know which type to use, such as:

1- The Java collections
2- The Reflection API.

## Exceptions in Java

**Exception** stands for “**Exceptional Event**”, which an event occurs during the program execution that disrupts the normal flow of the program

**Exception object** is object contains information about the error

**Throwing an exception** is creating an exception object and handing it to the runtime system

**Call stack** is a list of methods that the ordered methods that were called to get the method where the error occurred
exception handler is the block of code where error occurred

### The Catch or Specify Requirement

A code that might throw certain exceptions must be enclosed by either of the following:

- try statement that catches the exception which provide a handler for the exception

- A method that provides a throws clause that lists the exception

**The Three Kinds of Exceptions**

1- **checked exception**: exceptions that are well-written which means that the application can predict the exception (error) and solve it (recover)

     Checked exceptions are subject to the Catch or Specify Requirement.

2- **error**: exceptions that are externally and the application cannot predict the exception (error) and solve it (recover)

     Errors are not subject to the Catch or Specify Requirement.

3- **runtime exception**: exceptions that are internally and the application cannot predict the exception (error) and solve it (recover), usually indicate programming bugs, such as logic errors or improper use of an API

    Runtime exceptions are not subject to the Catch or Specify Requirement

## Scanning

The **objects of type scanner** useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

**By default, a scanner uses white space to separate tokens.**

- We need to close the scanner to indicate that user done with its underlying stream.

- Scanner also supports tokens for all of the Java language's primitive types (except for char)

**When using numeric values that use thousands separators, we need to mention the locale, because thousands separators and decimal symbols are locale specific**

**Resources**:

- [Java Primitives versus Objects](https://www.baeldung.com/java-primitives-vs-objects)
- [Exceptions in Java](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)
- [Scanning](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)
