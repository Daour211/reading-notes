## Java Imports

### Packages and Import:

Package is a directory. Java classes can be grouped together in packages.

The package (which contains the .java files) name is the same as the directory name.<br>
The user names the packages the he/she wants to use from other libraries in an import statement.

**Package declaration**
In a Java source file, the first statement is the package declaration and it is optional.
After the package declaration, I have the import statement which allow to specify classes from other packages that can be referenced without qualifying them with their package.

**Package declaration syntax**

The statement order is as follows:

1.  Package statement (optional).
2.  Imports (optional).
3.  Class or interface definitions.

- In the declaration I use The wildcard character (\*) is used to specify that all classes with that package are available to your program.

- Also in the declaration I can specify the class on the import statement.

- Another way is directly qualify the class without the need for import statement.

## Types of loops in Java

Looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

Types of loops that we can have in Java:

- Simple for loop: for loop allows to repeat certain operations by incrementing/decrementing and evaluating a loop counter.

- Enhanced for-each loop:

  - It starts with the keyword for like a normal for-loop.
  - Instead of declaring and initializing a loop counter variable, you declare a variable that is the same type as the base type of the array, followed by a colon, which is then followed by the array name.

  - In the loop body, you can use the loop variable you created rather than using an indexed array element.

- While loop: while loop repeats a statement or a block of statements while as long as the Boolean-expression is true.

- Do-While loop: do-while loop works just like the while loop except for that the code inside the loop is executed for one time before the condition evaluation

**Resources**:

- [Java Imports](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)

- [Types of loops in Java](https://www.baeldung.com/java-loops)
